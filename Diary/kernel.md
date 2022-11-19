<br>

vscode 에서 ipynb 확장자를 통해 Jupyter Notebook 을 쓸 수 있다.

그러나 Jupyter Notebook 내에 있는 코드를 실행 했을 때 

<br>

```py
failed to start the kernel. (code: 1073741845). bad file descriptor
```

<br>

위와 같은 에러가 뜨면서 실행이 안 되는 경우가 있다.

이는 Jupyter Lab 과의 충돌 때문인데,

다음과 같은 코드를 cmd 에 입력하자.

<br>

```py
pip uninstall pyzmq
```

<br>

그러면 y or n 을 입력하라는 메시지가 나오는데, 당연히 y 를 입력한다.

<br>

```py
pip install pyzmq==19.0.2
```

<br>

y 를 입력한 후 위와 같은 코드를 입력하면 에러가 해결된다 .. ^^
