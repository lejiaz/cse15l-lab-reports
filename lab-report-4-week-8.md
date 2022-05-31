our group: [link](https://github.com/alixintong/markdown-parser.git)
other group: [link](https://github.com/Shresthhooda/markdown-parser)
# Snippet 1
expected output
`[a link`](url.com)
[another link](`google.com)`
[`cod[e`](google.com)
[`code]`](ucsd.edu)
test code
[!image](1.jpg)

I believe that there definitely a small change that could fix my code for snippet 1. Case that the coder only  deal with a close bracket. Coding in a simple if statement checking that the next character is the last close bracket can cause the snippet one test to pass.


# Snippet 2
expected output
[a [nested link](a.com)](b.com)
[a nested parenthesized url](a.com(()))
[some escaped \[ brackets \]](example.com)
test code
[!image](2.jpg)
I also believe that there definitely a small change that could fix my code for snippet two. It is a case where the coder only has to deal with close brackets and close paren. Coding in two simple if statements checking that the next character is the last close bracket or last close paren can cause the snippet two test to pass.


# Snippet 3
expected output

[this title text is really long and takes up more than 
one line
and has some line breaks](
    https://www.twitter.com
)
[this title text is really long and takes up more than 
one line](
https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule
)
[this link doesn't have a closing parenthesis](github.com
And there's still some more text after that.
[this link doesn't have a closing parenthesis for a while](https://cse.ucsd.edu/
)
And then there's more text

test code
[!image](3.jpg)


# Test result
failed
1: [!image](11.png)
2: [!image](22.png)
3: [!image](33.png)

