I am not sure how github organizes folders or directories, but it should be laid out as follows.

Main_Directory

  docker-compose.yml
  Questions.txt

  client
    Dockerfile
    requirements.txt
    app
      client.py
  server
    Dockerfile
    requirements.txt
    app
      server.py
      
The code files provided include only one Dockerfile but the only thing that is different between
the two is the last line. In server it should be "./server.py" and in client it should be
"./client.py". There should also be two requirements.txt files but they are very short. In client
it should contain "requests" and in server it should contain "Flask". The questions.txt file
contains some basic questions and answers regarding Docker and how it works. 
