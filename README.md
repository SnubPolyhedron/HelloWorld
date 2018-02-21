package com.shu.datastructure;

public class ListStack <E>
{
	private LinkedList<E> list = new LinkedList<E>();
	
	/**
	 * 查看栈的大小
	 * @return
	 */
	public int size() 
	{
		return list.size;
	}
	
	/**
	 * 进栈操作
	 * @param e
	 */
	public void push(E e) 
	{
		list.add(e);
	}
	
	/**
	 * 出栈操作
	 * @return
	 */
	public E pop() 
	{
		E e = list.get(list.size - 1);
		list.delete(list.size - 1);
		return e;
	}
	
}
