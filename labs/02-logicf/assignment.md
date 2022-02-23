# Lab 2: Maksim Migulia

### 2-bit comparator

1. Karnaugh maps for other two functions:

   Greater than:

![image](https://user-images.githubusercontent.com/99403646/155404042-0675f57e-912d-4e3b-be15-f145423e1d85.png)

   Less than:

![image](https://user-images.githubusercontent.com/99403646/155404106-c97c9c3c-7dda-41d6-bbd0-24dc43b2c271.png)

2. Equations of simplified SoP (Sum of the Products) form of the "greater than" function and simplified PoS (Product of the Sums) form of the "less than" function.

 ![image](https://user-images.githubusercontent.com/99403646/155404138-804e3cfd-87f9-4b5a-996c-463970d6a6a9.png)

### 4-bit comparator

1. Listing of VHDL stimulus process from testbench file (`testbench.vhd`) with at least one assert (use BCD codes of your student ID digits as input combinations). Always use syntax highlighting, meaningful comments, and follow VHDL guidelines:

   Last two digits of my student ID: **xxxx??**

    p_stimulus : process
    begin
        -- Report a note at the beginning of stimulus process
        report "Stimulus process started" severity note;

           p_stimulus : process
    begin
        -- Report a note at the beginning of stimulus process
        report "Stimulus process started" severity note;

        -- First test case
        
        --INPUT PARAMETRS BY MY ID: 233261
                s_b <= "0110"; --6
                s_a <= "0001"; --1
                wait for 100 ns;
        assert ((s_B_greater_A = '1') and
                (s_B_equals_A  = '0') and
                (s_B_less_A    = '0'))
        report "Input combination 0110, 0101 FAILED" severity error;

        -- Report a note at the end of stimulus process
        report "Stimulus process finished" severity note;
        wait;
    end process p_stimulus;

2. Text console screenshot during your simulation, including reports.

   ![your figure]()

3. Link to your public EDA Playground example:

   [https://www.edaplayground.com/...](https://www.edaplayground.com/...)
