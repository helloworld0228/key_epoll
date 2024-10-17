# key_epoll
使用epoll方式读取键盘数据输入
原理
 epoll方式是应用在数据流方面的，比如在socket网络数据传输时候，数据传递就是流，当有数据过来的时候会触发。以同样的方式对于键盘和串口数据输入也是一种流，所以也可以检测数据输入。方便管理，不用使用一直读的方式去读取数据，改为被动式方式读取。
 
说明：

#define DEV_PATH1 "/dev/input/event4"
#define UART_DEVICE_NAME "/dev/ttyUSB1"
以上为键盘和串口控制句柄
