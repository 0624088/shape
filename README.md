```java
interface shape{
  // final double length=4;
  abstract void getArea();
}

class Rectangle implements shape{
  double length;
  double width;
  public Rectangle(double l,double w){
    length=l;
    width=w;
  }
  public void getArea(){
    System.out.println("Rectangle_area="+(length*width));
  }
}

class Triangle implements shape{
  double base;
  double height;
  public Triangle(double b,double h){
    base=b;
    height=h;
  }
  public void getArea(){
    System.out.println("Triangle_area="+(base*height/2));
  }
}

class Main {
  public static void main(String[] args) {
   Rectangle rect=new Rectangle(5, 10);
   rect.getArea();
   Triangle tri=new Triangle(5, 10);
   tri.getArea();
  }
}
```
