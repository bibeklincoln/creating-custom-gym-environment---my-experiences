# creating-custom-gym-environment---my-experiences


Creating custom env for own project in gym can be tidious, well, at least was for me. Here are brief descriptions of steps I used and finally created working custom gym environment.

1. Structure of project environment is one of the major issue:

![image] (https://user-images.githubusercontent.com/7438736/114192474-6f0f5100-9945-11eb-856b-a5fb0b5f0b94.png)


2. Assuming we are creating customEnv as custom gym environment, and so in the setup.py:

![image] (https://user-images.githubusercontent.com/7438736/114192654-a4b43a00-9945-11eb-845d-73c06aa58a1f.png)


3. The 1st __init__.py, should be like:

![image] (https://user-images.githubusercontent.com/7438736/114192986-ffe62c80-9945-11eb-9c2d-757faf5873af.png)


4. Then in the envs folder, the __init__.py should be like:

![image]https://user-images.githubusercontent.com/7438736/114193113-1d1afb00-9946-11eb-9de7-17a9a37d2556.png)


5. Finally the customEnv.py file should have following structure:

![image] (https://user-images.githubusercontent.com/7438736/114193269-43409b00-9946-11eb-9b62-6290522fb3d9.png)

- these 'render' and 'close' are optional. 

6. To complete the setup need to go back to the origin folder and run: pip3 install -e .  and following should happen:

![image] (https://user-images.githubusercontent.com/7438736/114193800-c8c44b00-9946-11eb-8704-126012866d83.png)

Yeah! we made it, aparently! 


