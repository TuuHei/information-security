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
* 

Readable at: https://owasp.org/Top10/A03_2021-Injection/

# a) Goat

First step is to install Java to our virtual machine using following lines:

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




