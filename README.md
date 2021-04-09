# creating-custom-gym-environment---my-experiences


Creating custom env for own project in gym can be tidious, well, at least was for me. Here are brief descriptions of steps I used and finally created working custom gym environment.

1. Structure of project environment is one of the major issue:

![image] file:///home/bibek/Pictures/1.png![image](https://user-images.githubusercontent.com/7438736/114194792-bf87ae00-9947-11eb-8e9e-5029b481b7b6.png)



2. Assuming we are creating customEnv as custom gym environment, and so in the setup.py:

![image] file:///home/bibek/Pictures/Screenshot%20from%202021-04-09%2014-57-11.png![image](https://user-images.githubusercontent.com/7438736/114194821-c6162580-9947-11eb-8100-dc331c773b7e.png)



3. The 1st __init__.py, should be like:

![image] file:///home/bibek/Pictures/Screenshot%20from%202021-04-09%2014-59-40.png![image](https://user-images.githubusercontent.com/7438736/114194756-b39bec00-9947-11eb-8bfd-23190a534cbc.png)



4. Then in the envs folder, the __init__.py should be like:

![image]file:///home/bibek/Pictures/Screenshot%20from%202021-04-09%2015-01-26.png![image](https://user-images.githubusercontent.com/7438736/114194844-cc0c0680-9947-11eb-8450-3df7bf880739.png)



5. Finally the customEnv.py file should have following structure:

![image] file:///home/bibek/Pictures/Screenshot%20from%202021-04-09%2015-04-29.png![image](https://user-images.githubusercontent.com/7438736/114194863-d29a7e00-9947-11eb-96a5-1ec7eb71c063.png)


- these 'render' and 'close' are optional. 

6. To complete the setup need to go back to the origin folder and run: pip3 install -e .  and following should happen:

![image] file:///home/bibek/Pictures/Screenshot%20from%202021-04-09%2015-17-00.png![image](https://user-images.githubusercontent.com/7438736/114194884-d7f7c880-9947-11eb-8224-8358a0c76c94.png)


Yeah! we made it, aparently! Now you update the customEnv.py as per your project to work on. 


