package com.company;

public class Main {

    public static void main(String[] args) {

        printer<Integer> a=new printer<Integer>(23);
        a.print();
        printer<String> b=new printer<String>("hello man!");
        b.print();


    }
}


class printer<T>
{
    T x;

    public printer(T x) {
        this.x = x;
    }

    public void print()
    {
        System.out.println("printing :"+this.x);
    }
}
