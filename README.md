public abstract class Kart {
    
    protected String name;
    protected String [][] anlamlar;
    
    public Kart(String name, String [][] anlamlar){
        
        this.anlamlar=anlamlar;
        this.name=name;
    }
    
    public String getName(){
        
        return this.name;
    }
    
    public abstract String[][] getAnlamlar();
    

    public String toString(){
        
        return ("Kart Ismi: "+name);
    }
}
