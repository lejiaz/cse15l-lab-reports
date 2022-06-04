# Streamlining ssh Configuration
my .ssh/config file
![image](config.png)
how I edit it
![image](editConfig.png)
command log in
![image](ieng6.png)
show scp command
![image](scp.png)
![image](output1.png)
![image](output2.png)

# Setup Github Access from ieng6
public key on Github and in user account
![image](scp.png)
keygen
![image](sshkey.png)
![image](keygit.png)
git commit
[link](https://github.com/lejiaz/cse15l-lab-reports/commit/8d01332e2c752e506d151fd240d38304ec40b924)
![image](gitcom.png)

# Copy whole directories with scp -r
![image](d.png)

`scp -r *.java *.md lib/ <hostname>:markdown-parse`

in one line:
`ls; cd markdownmarkdown-parser-main/; javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java; java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest;`
![image](md.png)


We can run multiple commands in one line using the `;` operand we will `scp` and `ssh` and run all in one go

`scp -r *.java *.md lib/ school:~/markdown-parse; ssh school "cd markdown-parse; /software/CSE/oracle-java-se-14/jdk-14.0.2/bin/javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java; /software/CSE/oracle-java-se-14/jdk-14.0.2/bin/java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest"`


