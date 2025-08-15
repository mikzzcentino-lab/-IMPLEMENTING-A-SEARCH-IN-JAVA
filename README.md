# -IMPLEMENTING-A-SEARCH-IN-JAVA

package myProjoct;


public class Main {

    public static void main(String[] args) {

        class Node implements Comparable<Node> {

            public int x, y;

            public double gCost, hCost;

            public Node parent;

            public Node(int x, int y) {

            }

             
            this.x  = x;

             
            this.y  = y;

            public double fCost() {

                return gCost + hCost;

            }

        
            public int compareTo(Node other) {

            }

            return Double.compare (

            this.fCost(), other.fCost());


            public boolean equals(Object obj) {

            }

            if (!(obj instanceof Node

            )) return false;

            Node other(Node)
            obj;

            return this.x
            == other.x && this.y  = other.y;

            @Override

            public int hashCode() {

                return Objects.hash(x, y);

                   public class AStarSearch {

                static int[][] grid = (
                
                        {0,0,0,0,0},
                        {0,0,1,0,0},
                        {0,0,1,0,0},
                        {0,1,0,0,0},
                        {0,0,0,0,0},
                                };

            Node current openSet.poll();

if (current.equals (goal) 
                ) {

List<Node> path new ArrayList<>();

                while (current  {
                    le 
                }
                null) path.add(current);

                current current.parent;

                Collections.reverse(path);

                return path;

                closedSet.add(current);

                for (int[] dir : new int[][][ {
                    (1
                }
                
                    ,0), (-1,0), (0,1), (0,-1))) { int nx current.x dir[
                    0], ny current
                    .y dir[
                    1]; if (nx >= 0 && ny >= 0 && nx < ROWS && ny < COLS && grid[nx][ny]  {
                        0
                    }
                    ) (

             Node neighbor new Node(nx, ny);
                    if (closedSet.contains(neighbor)) {
                        continue;
                    }

                    double tentative current.gcost + 1;

                    boolean better = false;

                    if (lopenSet.contains(neighbor)) {
                        (

       neighbor.hcost Math.abs(  nx goal.x) Math.abs(ny
                                - goal.y);
                    } else if (tentatived  {
                        neighbor.gCost
                    }) <

               better true;

              better true;

              If(better) (

                 neighbor.gCost tentatives;

                    neighbor.parent current;

                    openSet.add(neighbor);
                                
                                      
                                
                
                
            }

        }


                                
            }

        }













import java.util.*;


class Node implements Comparable<Node>{

    public int x, y;
    public double gCost, hCosh;
    public Node parent;
    
    
    
    public Node(int x, int y){
        
        this.x = x;
        this.y= y;
    }
    
    
    
    public double fCost (){
        return gCost + hCosh;
    }
  
    @Override
    public int compareTo(Node other) {
        return Double.compare(this.fCost(),other.fCost());
    }
    
    
    
    @Override
    public boolean equals(Object obj){
       if (!(obj instanceof Node))return false; 
       Node other =(Node)obj;
        return this.x == other.x && this.y == other.y;
        
   
        
    }
    
    @Override 
    public int hashCode(){
        return  Objects.hash(x, y);
         
    }
} 
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
