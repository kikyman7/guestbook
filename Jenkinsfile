AKIA3TEBY2US2RLMJ7WJ

k0KROliSUyeb54nDKdDSITghuPjCEwmYIyKRWXG7

controller_public-ip = "43.200.152.128"

Jenkins
http://43.200.152.128:8080

parse_git_branch() {
	git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}
export PS1="[\u@\h \[\033[32m\]\W\[\033[33m\]\$(parse_git_branch)\[\033[00m\]]# "

gitHub Token
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

git remote add origin https://github.com/kikyman7/guestbook.git

sonarqube
http://13.125.112.6:9000

guestbook-token: b01612acf7c6eec671e973bd46daac6543f35a3e

http://43.200.152.128:8080/sonarqube-webhook/

mvn sonar:sonar \
  -Dsonar.projectKey=guestbook \
  -Dsonar.host.url=http://13.125.112.6:9000 \
  -Dsonar.login=b01612acf7c6eec671e973bd46daac6543f35a3e
  
stage
http://43.201.112.171:38080

# index.html 수정
cd ~/lab/projects/guestbook
vi src/main/resources/templates/index.html

git add .
git commit -m "[UPDATE] index.html"

git push origin master

# jmeter 스크립트 형상관리
cp /root/lab/sw/guestbook_loadtest.jmx /root/lab/projects/guestbook/src/main/jmx/guestbook_loadtest.jmx
cd ~/lab/projects/guestbook
git add .
git commit -m "[ADD] LOAD TEST"
git push origin master

