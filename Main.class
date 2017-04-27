import java.util.*;
import java.io.*;
class WeightedChooser {
	private ArrayList<Integer> weighted;
	WeightedChooser(ArrayList<Integer> options, ArrayList<Integer> weights) {
		this.weighted = new ArrayList<Integer>();
		for(int i=0;i<options.size();i++) {
			for(int j=0;j<weights.get(i);j++) {
				this.weighted.add(options.get(i));
			}
		}
	}
	public int choose() {
		return this.weighted.get((int)(Math.random()*this.weighted.size()));
	}
}
class Main {
  public static void main(String[] args) {
    ArrayList<Integer> c = new ArrayList<Integer>();
    c.add(1);c.add(2);c.add(3);
    ArrayList<Integer> w = new ArrayList<Integer>();
    w.add(1);w.add(2);w.add(3);
    WeightedChooser wc = new WeightedChooser(c,w);
    for(int i = 0;i < 20;i++) {
      System.out.println(wc.choose());
    }
  }
}
