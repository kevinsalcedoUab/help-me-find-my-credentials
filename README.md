# Help me find my SSH credentials

We have a problem. Our devops cowoer messed up a little the information about our credentials to connect to the production server.

He veguely rememebers some clues that may help us to find our way to connect to the remote server in Amazon Web Services.

## Objective

We should be able to retrieve two pieces of information

1. We need to discover which is our username in the remote server
2. We need to figure out which [PEM file](https://s3.amazonaws.com/smhelpcenter/smhelp941/classic/Content/security/concepts/what_are_pem_files.htm) do we need to use to connect to our server 

```
ssh -i "correct-certificate-file.pem" correct-username@ec2-35-181-5-201.eu-west-3.compute.amazonaws.com
```

To prove that you were able to connect, create a txt file with your name.

Once you are able to connect, you should be able to see:

<img src="https://oscarm.tinytake.com/media/fa5eb0?filename=1617172318207_TinyTake31-03-2021-08-31-00_637527691184865337.png&sub_type=thumbnail_preview&type=attachment&width=669&height=154" title="Powered by TinyTake Screen Capture"/><br><a href="https://www.tinytake.com">Powered by TinyTake Screen Capture</a>

## Username

Bob, our devop coworker, remebers that our "corrrect-username" is somewhere in a TXT file in this folder or subfolders. Maybe a terminal command could help us to search for all these types of files. He also mentions that the name of the file is in a beautiful language. We think we may have to look inside the file using a command in order to filter the text lines to find our username.

BONUS: Which is the novel that this TXT file contains?

## PEM file

Again, Bob does not remember where is the correct PEM file. "Somewhere in this folder!" - he says. Not very helpful. He also mentions that:

* Ineed, it MUST be a PEM file
* If you find more that one PEM file, I think that the correct one is about 2K size.


