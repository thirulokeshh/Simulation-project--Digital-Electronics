# TITLE:
Minimise the function using K map F(A,B,C)=A′BC+A′BC′+AB′C′+AB′C and simulate the logic diagram using verilog


# THEORY:
The K-map is a systematic way of simplifying Boolean expressions. With the help of the K-map method, we can find the simplest POS and SOP expression, which is known as the minimum expression. The K-map provides a cookbook for simplification.

Just like the truth table, a K-map contains all the possible values of input variables and their corresponding output values. However, in K-map, the values are stored in cells of the array. In each cell, a binary value of each input variable is stored.

The K-map method is used for expressions containing 2, 3, 4, and 5 variables. For a higher number of variables, there is another method used for simplification called the Quine-McClusky method. In K-map, the number of cells is similar to the total number of variable input combinations. For example, if the number of variables is three, the number of cells is 23=8, and if the number of variables is four, the number of cells is 24. The K-map takes the SOP and POS forms. The K-map grid is filled using 0's and 1's. The K-map is solved by making groups. There are the following steps used to solve the expressions using K-map:

# LOGIC DIAGRAM:
<img width="580" alt="Screenshot 2023-05-30 203337" src="https://github.com/thirulokeshh/Simulation-project--Digital-Electronics/assets/124516517/e77d1c81-0eec-4305-978b-9ae07af5e619">


# NETLIST DIAGRAM:
<img width="650" alt="Screenshot 2023-05-30 190827" src="https://github.com/thirulokeshh/Simulation-project--Digital-Electronics/assets/124516517/16cb3184-54cf-4336-986c-92f11aff923c">


# TIMING DIAGRAM:
![Screenshot (27)](https://github.com/thirulokeshh/Simulation-project--Digital-Electronics/assets/124516517/efdf102a-000c-4be9-b409-bc5fa84545a8)



# PROGRAM:
~~~
module assignment(A,B,F);
input A,B;
output F;
xor(F,A,B);
endmodule
~~~

# REFERENCE:
https://www.javatpoint.com/karnaugh-map-in-digital-electronics
