A simple HTML5 client and server integrated with AWS Polly
-------------------------------------------------------

The following is an example provided by AWS on their docs site [here](http://docs.aws.amazon.com/polly/latest/dg/examples-python.html).

The below is a quick guide and how to get set up.

# Set up virtualenv

Install virtualenv

```
pip install virtualenv
```

Create a virtualenv environment
```
virtualenv env
```

Activate a new virtualenv environment

```
source env/bin/activate
```

# Install dependenciesssa

e.g.

```
pip install boto3
```

# Modify code to use your AWS profile

Modify the following snippet of code to specify your aws profile,
typically stored in your ~/.aws/credentials file. In this case I used a
profile called polly.

```
session = Session(profile_name="polly")
```

# Start Server

```
http://localhost:8000/index.html
```

# Open browser

```
open http://localhost:8000/index.html
```

Select your voice, type your text, and hear the response!

Note: At the time of writing this is only available in selected regions
