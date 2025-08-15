# -IMPLEMENTING-A-SEARCH-IN-JAVA

package myProjoct;

import java.util.*;

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
            }

        }
