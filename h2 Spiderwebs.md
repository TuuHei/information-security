# x) Read and summarize

## Security Misconfiguration

* It is  critical to keep software updated and enabled.
* If default accounts and their passwords aren't disabled or changed, attackers can log in with the default passwords.


Readable at: https://owasp.org/Top10/A05_2021-Security_Misconfiguration/

## Vulnerable and Outdated Components.

* Was #2 on the community OWASP survey.
* It is a harder gategory to test and calculate risks.
* It is critical to know the versions of components in use and actively research if there are known vulnerabilities with them.
* Getting components from official sources over secure links is adviced.
* As components typically run with the same privileges as the application, component flaws can result in serius impact.

Readable at: https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/

## Injection

* More common injections are SQL, NoSQL, OS command, Object Relational Mapping (ORM), LDAP and Expression Language (EL).
* Best method for detecting if applications are vulnerable is source code review.

Readable at: https://owasp.org/Top10/A03_2021-Injection/

# a) Goat

First step is to install Java to our virtual machine using these commands:

$ sudo apt-get update

$ sudo apt-get -y install openjdk-17-jre ufw wget bash-completion

I also enabled fire wall using:

$ sudo ufw enable

![kuva](https://github.com/TuuHei/information-security/assets/122973223/9ebaff55-b612-440d-9017-1c15532c6adf)

Next step is to install and register to Webgoat.

I put these commands to the terminal:

$ wget https://terokarvinen.com/2020/install-webgoat-web-pentest-practice-target/webgoat-server-8.0.0.M26.jar

$ java -jar webgoat-server-8.0.0.M26.jar

![kuva](https://github.com/TuuHei/information-security/assets/122973223/17f82611-12d0-4b51-9975-33aee7e5a29f)

# b) F12. Solve Webgoat 8: General: Developer tools.

After installing WebGoat I registered there and started the Developer tools exercises.

Firstly I looked into developer tools and ran a couple commands there.

![1](https://github.com/TuuHei/information-security/assets/122973223/b996b79b-338b-429c-8782-691249277b57)

First assignment was to retrieve a random number using a command in the developer tools console.

![2](https://github.com/TuuHei/information-security/assets/122973223/07d95772-15df-4850-98e5-73cb23660e10)

The second and last assignment was to find a number from a HTML request.

![3](https://github.com/TuuHei/information-security/assets/122973223/50ae9752-4a97-4312-badf-52b81eee3ccb)

# c) Not outdated. Update all operating system and all applications in your Linux.

To update the operating system and its applications I used these commands in the terminal:

$ sudo apt-get update

$ sudo apt-get -y dist-upgrade

# d) Sequel. Solve SQLZoo

I solved some SQL tasks using SQLZoo. Firstly 0 SELECT basics part, where there were 3 tasks.

I only had to change the part where it showed 'France' to 'Germany'.

![5](https://github.com/TuuHei/information-security/assets/122973223/49ab46d7-f943-4f11-9680-4fff32421e0c)

This was also a task where I only changed the countries as instructed.

![6](https://github.com/TuuHei/information-security/assets/122973223/2655893b-9028-4758-b37d-9c0b4f793e4e)

I modified the numbers to their right values.

![7](https://github.com/TuuHei/information-security/assets/122973223/ed8e7e9a-4542-4db6-a112-a9c97fb887e6)

Second part was to complete 2 first subtasks from 2 SELECT from world.

I had to find countries from the table world, where the population is more than 200 million.

![8](https://github.com/TuuHei/information-security/assets/122973223/cc9a8767-e0d7-4210-b1f2-1614185ff320)

In the last task I had to calculate per capita GDP, where population is more than 200 million.

![9](https://github.com/TuuHei/information-security/assets/122973223/cc384392-44bf-43f6-897d-f88fb8b567d7)

# Johnny tables. Solve Portswigger Labs

The task is to retrieve hidden data from an online shop. First thing I did on the website was to choose a gategory
and then simply type '-- after the URL. The site then showed one more product than previosly.

![kuva](https://github.com/TuuHei/information-security/assets/122973223/92679e23-f468-43ac-8e75-df0aeea08e97)

![kuva](https://github.com/TuuHei/information-security/assets/122973223/c1b011ff-9422-4aa6-9cb5-6225876c2204)

To show even more products, I put '+OR+1=1-- after the URL. This was a helpful website druing this exercise: https://owasp.org/Top10/A03_2021-Injection/

![kuva](https://github.com/TuuHei/information-security/assets/122973223/2fdc9d00-466b-483f-862e-d9585330d304)
