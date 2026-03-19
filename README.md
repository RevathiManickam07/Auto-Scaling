# Auto-Scaling
Highly Available Web Application Deployment using Auto Scaling

# 🔹 What is Auto Scaling?

Auto Scaling is a cloud feature that automatically adds or removes resources (like EC2 instances) based on demand.

👉 In AWS, it is called Amazon EC2 Auto Scaling

# 🔹 Why do we use Auto Scaling?

*To handle high traffic automatically

*To avoid server crashes

*To save cost when traffic is low

# 🔹 How it works:
1.You define minimum, desired, and maximum instances

2.Set scaling policies (CPU usage, traffic, etc.)

3.AWS automatically:

     Adds instances → when load increases 📈
     
     Removes instances → when load decreases 📉

# 🔹 Advantages of Auto Scaling

   1.High Availability
   2.Cost Optimization
   3.Better Performance
   4.Fault Tolerance
   5.Scalability
#🔹 Real-Time Use Cases

   1.E-commerce Websites (Flipkart / Amazon)
   2.Healthcare Application
   3.OTT Platforms (Netflix)
   4.Banking Applications

# Practical steps to create auto scaling in aws:

# step 1:Create Target Group

![Image Alt](https://github.com/RevathiManickam07/Auto-Scaling/blob/d3d4259d42c450ccffdb2fe4f85cabcc66952ca3/Create%20Target%20Group.PNG)    

# 🔹 Step 2: Create Load Balancer (ALB)

![Image Alt](https://github.com/RevathiManickam07/Auto-Scaling/blob/be7bc5cb6de7b8238ee42f26886dbb96c4f8fc18/Create%20Load%20Balancer%20(ALB).PNG)   

# 🔹 Step 3: Create Security Group

![Image Alt](https://github.com/RevathiManickam07/Auto-Scaling/blob/c0ee817a93afe1db7a7c4d535c469a6d777aa806/Create%20security%20group.PNG)    


# 🔹 Step 4: Create Launch Template

![Image Alt](https://github.com/RevathiManickam07/Auto-Scaling/blob/b5e71ed928f774497f21a3da94acbdea88353810/Create%20Launch%20Template.PNG)   


# User Data

```bash
#!/bin/bash
yum update -y
yum install httpd -y
systemctl start httpd
systemctl enable httpd
```

# 🔹 Step 4: Create Auto Scaling Group (ASG)
![Image Alt](https://github.com/RevathiManickam07/Auto-Scaling/blob/84a9c18aad2c4690e0b98f9802fd9a900931c819/Create%20Launch%20Template.PNG)  




# 🔹 Step 5: Final output of the Autoscaling Project

![Image Alt](https://github.com/RevathiManickam07/Auto-Scaling/blob/685796eafd713fcbd7b572fdc0a2e81d4ea17458/Ec2%20instance%20created%20using%20ASG.PNG)   

![Image Alt](https://github.com/RevathiManickam07/Auto-Scaling/blob/685796eafd713fcbd7b572fdc0a2e81d4ea17458/Final%20output.PNG)    

# Conclusion 

“In this project, I implemented an Auto Scaling Group with a Load Balancer to achieve high availability and scalability. The system automatically scales EC2 instances based on demand, ensures fault tolerance, and optimizes cost by running only required resources.”


