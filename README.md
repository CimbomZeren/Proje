# Proje

package ılkprogram;

public class Circle extends GeometricObject {
    
    private double radius;
    
    public Circle(double radius){
        
        this.radius=radius;
    }
    
    public double getRadius(){
        
        return this.radius;
    }
    
    public void setRadius(double radius){
        
        this.radius=radius;
    }
    
    public double getArea(){
        
        double alan;
        
        alan=radius*radius*(Math.PI);
        return alan;
    }
    
    public double getPerimeter(){
        
        double cevre;
        
        cevre=2*radius*(Math.PI);
        return cevre;
    }
    
    public double getDiameter(){
        
        return radius*2;
    }
}
