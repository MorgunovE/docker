1. https://www.docker.com/
2. download
3. install
4. install docker plugin in vscode and webstorm
5. add index.py
6. add  and code
7. docker build .
8. docker image ls
9. docker run 3b4ddd31d355 //from docker image ls
10. docker hub node google https://hub.docker.com/_/node
11. docker pull node
12. docker images
13. docker run node
14. docker ps --help
15. docker run --help
16. docker ps
17. docker ps --help
18. docker ps -a
19. docker run -it node
20. docker ps -a
21. docker rm 09d0d8230556
22. docker rm 98368c1e0e05 73d6643c1aeb
23. docker container prune
24. clone https://github.com/vladilenm/logs-app.git
25. cd logs-app
26. npm i
27. ////////// now working in logs-app
28. add Dockerfile and code
29. docker build .
30. docker images
31. id d2ad958b4709
32. docker run d2ad958b4709
33. docker ps in new terminal
34. docker stop ae0f23fa34ea //id container
35. docker ps
36. docker ps -a
37. docker start ae0f23fa34ea //id container
38. docker ps
39. docker images
40. docker run -p 3000:3000 d2ad958b4709
41. docker ps
42. docker stop 06572fd57a12
43. docker ps -a
44. docker run -d -p 80:3000 d2ad958b4709
45. docker ps
46. docker stop pensive_burnell //names
47. docker ps -a
48. docker start pensive_burnell
49. docker stop pensive_burnell
50. docker ps
51. docker ps -a
52. docker container prune // y
53. docker images
54. docker run -d -p 3000:3000 d2ad958b4709
55. add code in app.js
56. change code in index.ejs
57. docker ps
58. docker stop 6c0ef5c299ad
59. docker build .
60. docker images
61. docker run -d -p 3000:3000 03daf01f7fa5
62. docker ps
63. docker stop angry_fermi
64. add code in Dockerfile COPY package.json /app and change place for RUN npm install
65. docker build .
66. docker images
67. docker run -d -p 3000:3000 460bc30eede9
68. docker ps
69. docker stop 434f820bd0dc
70. docker images
71. docker run -d -p 3000:3000 460bc30eede9
72. docker ps
73. docker attach 423794eb16d8
74. docker logs 423794eb16d8
75. docker images
76. docker run -d -p 3000:3000 --name logsapp 460bc30eede9
77. docker logs logsapp
78. docker stop logsapp
79. docker ps -a
80. docker container prune
81. docker ps -a
82. docker images
83. docker run -d -p 3000:3000 --name logsapp --rm 460bc30eede9
84. docker ps
85. docker stop logsapp
86. docker ps
87. docker ps -a
88. docker images
89. docker rmi d2ad958b4709 03daf01f7fa5
90. docker images
91. docker image prune
92. docker images
93. docker build -t logsapp .
94. docker images
95. docker run -d -p 3000:3000 --rm logsapp
96. docker ps
97. docker stop 28223e9a6f86
98. add code in index.ejs
99. docker build -t logsapp:exl .
100. docker images
101. docker run -d -p 3000:3000 --rm --name logsapp logsapp:exl
102. docker stop logsapp
103. docker run -d -p 3000:3000 --rm --name logsapp logsapp
104. docker stop logsapp
105. docker rmi logsapp:exl
106. docker images
107. sing up in docker for docker hub
108. docker login
109. docker images
110. docker tag logsapp morgunove/logsapp
111. docker images
112. docker push morgunove/logsapp:latest
113. docker images
114. docker rmi logsapp morgunove/logsapp
115. docker images
116. docker pull morgunove/logsapp
117. docker images
118. docker run -d -p 4200:3000 --rm --name logsapp morgunove/logsapp
119. docker stop logsapp
120. add .dockerignore
121. docker rmi morgunove/logsapp
122. docker images
123. docker build -t logsapp .
124. docker images
125. docker image inspect logsapp
126. add PORT in Dockerfile
127. docker build -t logsapp:env .
128. docker images
129. docker run -d -p 3000:4200 --rm --name logsapp logsapp:env
130. docker stop logsapp
131. docker run -d -p 3000:80 -e PORT=80 --rm --name logsapp logsapp:env
132. docker logs logsapp
133. docker stop logsapp
134. add config .env and code
135. docker run -d -p 80:4200 --env-file ./config/.env --rm --name logsapp logsapp:env
136. docker logs logsapp
137. docker stop logsapp