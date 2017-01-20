###Standing Up a Server

The goal of the exercises today is to stand up an http server on Amazon Web Services [AWS]. An http server is a computer (real or virtual) that exists for the simple purpose of handling requests over the http protocol from web browsers and other access points.

When web browsers type in a domain name, DNS services convert that domain name into an IP address, and the computer's request is routed to the server associated with that address. Depending on the content and settings on the server, the server then performs actions and returns results to the requesting machine. 

Servers are no different from the computer that we use every day, except that they are often `headless`, and lack any kind of display or input. Instead, they sit in stacks of hundreds of identical machines in air conditioned `datacenters` in locations where real estate is cheap. Each physical machine can also be partitioned into several virtual machines, so that many users can use the resources of each server and determine their own configurations

![datacenter](http://datacenterfrontier.com/wp-content/uploads/2015/09/amazon-dc-hamilton.jpg)

Amazon offers services via AWS that powers the servers and other parts of the technology stack of a significant proportion of the internet. We are using it in class because of its free tier and genericness, but other options are available such as the recommendable [Dreamhost](http://www.dreamhost.com) and [HostGator](http://www.hostgator.com). [Google Cloud Computing](http://cloud.google.com) is a competing service as well that offers more power at the cost of complexity.


- Visit http://www.aws.amazon.com.
- Create an account on AWS.
- Login to see the AWS dashboard. 
- Visit the Services menu, and under the `Compute` menu, select `EC2`.
- Click the `Launch Instance` button.

AWS will then offer you options for which operating system to install on the virtual server


