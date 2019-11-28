```java
interface shape{
  abstract void getArea();
}

class Rectangle implements shape{
  double length;
  double width;
  String shapename1;
  String Rectangle_area;
  public Rectangle(double l,double w,String SN1){
    length=l;
    width=w;
    shapename1=SN1;
  }
  public void getArea(){
    Rectangle_area=("Rectangle_area="+(length*width));
  }
  public String toString(){
  return Rectangle_area+""+shapename1;  
 }  
}

class Triangle implements shape{
  double base;
  double height;
  String shapename;
  String Triangle_area;
  public Triangle(double b,double h, String SN){
    base=b;
    height=h;
    shapename=SN;
  }
  public void getArea(){
  
  Triangle_area=("Triangle_area="+(base*height/2));
  }
  public String toString(){
  return Triangle_area+""+shapename;  
 }  
}


class Main {
  public static void main(String[] args) {
   Rectangle rect=new Rectangle(5, 10,"  RectangleArea");
   rect.getArea();
   System.out.println(rect);
   Triangle tri=new Triangle(5, 10,"  TriangleArea");
   tri.getArea();
   System.out.println(tri);
  }
}
```
