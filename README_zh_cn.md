dumb-init
========

[![Travis CI](https://travis-ci.org/Yelp/dumb-init.svg?branch=master)](https://travis-ci.org/Yelp/dumb-init/)
[![PyPI version](https://badge.fury.io/py/dumb-init.svg)](https://pypi.python.org/pypi/dumb-init)

**dumb-init** 是一个简单的进程管理和和系统初始化工具，扮演最小化容器运行环境里的PID为1的init进程  (例如[Docker][docker])。 
它是用C语言编写，体积微小的静态链接二进制程序

轻量级容器通常作为单一进程和服务来运行，没有使用类似[systemd][system]或[sysvinit][sysvinit]这样的初始化系统工具，
导致不能正常的处理进程信号。引起容器优化
