# Description
This started out as a small project to help me to learn Python and has now grown into a fully working API service. I had a requirement to create temporary SFTP access accounts that would expire after a few days, this API was created to take away the burden of management and my forgetfulness to remove accounts!

# Running in Production
You can run this in production, however, you must test and configure the host to best practices. This code has not been security tested and it is up to you to ensure it is safe for your environment. I personally run this over HTTPS and recommend you do the same, additionally, I have only allowed TLS 1.2 with strong cyphers.

# Setup
```
sudo su
wget -O - -q https://raw.githubusercontent.com/OneLogicalMyth/sftp-service/master/setup.sh | bash
```

Note: At times the pip install seems to fail for reasons unkown ensure that flask and requests is installed if you notice any pip install errors during the scripts execution; this can be done by running:
```
pip install Flask
pip install requests
```

Once installed you can then start making use of the API using curl or any application you have developed to work with it.
