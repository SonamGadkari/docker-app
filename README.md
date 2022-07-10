This is project referred from in28min as a part of exploring microservices.

<h4>Generate jar:</h4>
<li>Using Maven install in any IDE</li>

<h4>Generate docker image:</h4>
<p> &nbsp; &nbsp; Go to the project root directory, for ex: C:\currency-exchange-service, Using the below command
    <li> docker run -f Dockerfile -t NewDockerImageNameForCreation . </li>
</p>

<h4>Push repo to docker hub </h4>
<p> &nbsp; &nbsp; Before pushing the repo , generate tag using the below command
    <li> docker tag NewDockerImageNameForCreation DockerRepoPath/NewDockerImageNameForCreation </li>
    <p> for ex: docker tag docker-currency-exchange sonamgadekari/docker-currency-exchange</p>
    <p> Actual command to push the repo to docker hub </p>
    <li> docker push sonamgadekari/docker-currency-exchange</li>
</p>

<h4>Pull repo from docker hub</h4>
<p>docker pull sonamgadekari/docker-currency-exchange</p>
   
<h4>Run app in docker container:</h4>
<p> &nbsp; &nbsp; Using the below command
    <li> docker run -p 8000:8000 -d docker-currency-exchange </li>
</p>
