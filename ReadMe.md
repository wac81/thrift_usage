# thrift usage in python 2.7

### base on:
http://tkang.blogspot.com/2010/07/thrift-server-client-in-python.html

## 1.you install thirft at first:
use
pip install thirft
or
http://thrift-tutorial.readthedocs.io/en/latest/installation.html

## 2.you can generate gen-py by yourself use below:
thrift --gen py helloworld.thrift

### you can use helloworld.thrift below

const string HELLO_IN_KOREAN = "an-nyoung-ha-se-yo"
const string HELLO_IN_FRENCH = "bonjour!"
const string HELLO_IN_JAPANESE = "konichiwa!"

service HelloWorld {
  void ping(),
    string sayHello(),
    string sayMsg(1:string msg)
}


## 3.then you can start server and client like that:
python helloserver.py
python helloclient.py


## 4.you can know about JAVA example here:
http://thrift-tutorial.readthedocs.io/en/latest/usage-example.html#java-multiplication-server





