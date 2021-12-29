# Sherlock-Homes


import java.io.BufferedReader;
import java.io.InputStreamReader;
 
 

class P8
{
    public static void main(String args[] ) throws Exception {
       BufferedReader sherlock = new BufferedReader(new InputStreamReader(System.in));
	
		int t = Integer.parseInt(sherlock.readLine());
		StringBuilder nikhil = new StringBuilder();
 
		while(t-->0){
			String s1 = sherlock.readLine();
			String s2 = sherlock.readLine();
			
			boolean bool=false;;
			
			if(s2.contains(s1)){
				bool=true;
			}
			s1 = new StringBuilder(s1).reverse().toString();
			if(s2.contains(s1)){
				bool=true;
			}
			
			if(bool){
				nikhil.append("YES\n");
			}
			else{
				nikhil.append("NO\n");
			}
		}
		System.out.print(nikhil);
    }
}	

