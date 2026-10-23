# Challenge: Install It Yourself

1. Install http, run it, write one thing it shows.
   Commands: http   ->   sudo apt install -y httpie   ->   http
   It shows: "HTTPie - a CLI, cURL-like tool for humans" (usage line).

2. Which version of apache2 does Ubuntu offer? (not installed)
   Command: apt show apache2 | head - 4
   Answer: Version: 2.4.58-1ubuntu8

3. How many packages are installed now?
   Command: apt list --installed | wc -l
   Answer: 780

4. Docker alpine prints Hello from Alpine.
   Command: sudo docker run --rm alpine echo Hello from Alpine
   Output: Hello from Alpine

5. Docker key file and sources file full paths.
   Commands: ls -l /etc/apt/keyrings/ ; ls /etc/apt/sources.list.d/
   Key:     /etc/apt/keyrings/docker.asc
   Sources: /etc/apt/sources.list.d/docker.sources

6. Remove http and prove it is gone.
   Commands: sudo apt remove -y httpie ; hash -r ; http
   Proof: http -> "Command 'http' not found, but can be installed with: ..."
