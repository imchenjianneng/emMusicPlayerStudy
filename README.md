# emMusicPlayerStudy
简易音乐播放器  
    &emsp;&emsp;很多时候我们都会用手机来播放音乐，播放视频，那么具体地要怎么实现呢，其实主要是MediaPlayer类来完成的。下面通过简单的例子来实现一首歌曲的播放吧。新建工程MediaPlayerStudy，这里我们来简单地实现个音乐播放器，首先来简单布局下：见工程。  
    &emsp;&emsp;这里button没有使用imagebutton，方便起见，ui就都利用现有的资源了，以后再改进。播放的列表也不实现了，简单地实现播放，暂，seek，还有总时间显示，进度显示等功能，基本上除了上下曲，一个简单地音乐播放器也完成了。下面看下代码：见工程。  
    &emsp;&emsp;对于按键的监听就不多说了，这里还学了seekbar，seekbar的话其实和一般的也差不多。当seek的点改变的时候，那么就会调用onProgressChanged，当拖动的时候手指还没有弹起的时候调用onStartTrackingTouch，当拖动手指弹起的时候调用onStopSTrackingTouch。  
    &emsp;&emsp;这里通过MediaPlayer来调用播放音乐，其中setDataSource是指定播放器播放的路径，然后prepare准备好，接着start启动，pause暂停等
等。具体就不展开了。  
    &emsp;&emsp;这里使用了thread线程还有handler，因为线程中不能更改ui，所以必须用handler等去实现，具体以后再说吧。  
    &emsp;&emsp;运行可以按播放，播放音乐，然后暂停可以暂停播放，拖动进度条，可以到指定的时间去播放，并且时间也会走。简单的音乐播放器就这么多了，之后有机会再好好完善播放列表，音量啊，音频的一些资源显示等，像qq音乐啊，酷狗啊，都很不错，可以模仿模仿。  
    
