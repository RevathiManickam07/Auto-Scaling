# Auto-Scaling
Highly Available Web Application Deployment using Auto Scaling

#🔹 What is Auto Scaling?
Auto Scaling is a cloud feature that automatically adds or removes resources (like EC2 instances) based on demand.

👉 In AWS, it is called Amazon EC2 Auto Scaling

#🔹 Why do we use Auto Scaling?
*To handle high traffic automatically
*To avoid server crashes
*To save cost when traffic is low

#🔹 How it works:
1.You define minimum, desired, and maximum instances

2.Set scaling policies (CPU usage, traffic, etc.)

3.AWS automatically:
     Adds instances → when load increases 📈
     Removes instances → when load decreases 📉

#🔹 Advantages of Auto Scaling
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


# 🔹 Step 2: Create Load Balancer (ALB)



# 🔹 Step 3: Create Security Group



# 🔹 Step 4: Create Launch Template



"" User Data  ""

''' #!/bin/bash
yum update -y
yum install httpd -y
systemctl start httpd
systemctl enable httpd
echo "Hello from Auto Scaling Instance" > /var/www/html/index.html'''

