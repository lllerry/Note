## 栈

### 链表实现

```
public class Stack<T> {

    static class NodeV<T> {
        T t;
        NodeV mNext;
    }

    //栈顶
    NodeV first;
    //索引
    int index;

    //压栈
    public void push(T t) {
        //向栈顶添加元素
        NodeV oldNode = first;
        first = new NodeV();
        first.t = t;
        first.mNext = oldNode;
        index++;
    }

    //出栈
    public T pop() {
        T t = (T) first.t;
        first = first.mNext;
        index--;
        return t;
    }

    public boolean isEmpty() {
        return index == 0;
    }

    public int size() {
        return index;
    }
}
```

### 数组实现

```
public class FixedCapacityStack<T> implements Iterable<T> {
    private T[] container;
    //索引
    private int index;

    public FixedCapacityStack(int cap) {
        container = (T[]) new Object[cap];
    }

    //进栈
    public void push(T content) {
        //判断栈是否已满
        if (index == container.length) {
            resize(2 * container.length);
        }
        container[index++] = content;
    }

    //弹栈
    public T pop() {
        if (index == 0) {
            throw new IllegalStateException("you can't do this");
        }

        //如果数据的长度小于
        T result = container[--index];
        container[index] = null;
        if (index > 0 && index == container.length / 4) {
            resize(container.length / 2);
        }
        return result;
    }

    public boolean isEmpty() {
        return index == 0;
    }

    public int size() {
        return index;
    }


    private void resize(int max) {
        T[] temp = (T[]) new Object[max];

        for (int i = 0; i < index; i++) {
            temp[i] = container[i];
        }
        container = temp;
    }

    @Override
    public Iterator<T> iterator() {
        return new ReverseArrayIterator<>(container);
    }
}

public class ReverseArrayIterator<T> implements Iterator<T> {

    private int index;
    private T[] mContainer;

    public ReverseArrayIterator(T[] container) {
        mContainer = container;
        index = mContainer.length;
    }

    @Override
    public boolean hasNext() {
        return index > 0;
    }

    @Override
    public T next() {
        return mContainer[--index];
    }
}
```