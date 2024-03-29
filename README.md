
<div id="top"></div>
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="#">
    <img src="https://imgs.search.brave.com/Xftt8kk2m5f-q7wfrFC45rKBq7j4wZlIAX6iji82T3o/rs:fit:1023:369:1/g:ce/aHR0cHM6Ly9mYXN0/YXBpLnRpYW5nb2xv/LmNvbS9pbWcvbG9n/by1tYXJnaW4vbG9n/by10ZWFsLnBuZw" alt="Logo">
  </a>

  <h3 align="center">FastyAPI</h3>

  <p align="center">
    A FastAPI based Stack boilerplate for heavy loads.
    <br />
    <a href="#"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="#">View Demo</a>
    ·
    <a href="#">Report Bug</a>
    ·
    <a href="#">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#environment-setup">Environment setup</a></li>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#running-and-testing">Running and testing</a></li>
      </ul>
    </li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

FastyAPI is a FastAPI based Stack boilerplate designed for heavy workloads and simple developement in mind.

Here's why:
* FastAPI provides such a great developement experience due to its simple structure and the auto generated docs.
* we've improves this further by providing you with a simple design pattern, no subfolders <3
* every Stack element is carefully chosen and tested/optimised against heavy workloads
* boiletplate code for different situations, websocket, crud etc.. yet without bloat.

<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

Our stack is as follows
* [Gunicorn](https://fastapi.tiangolo.com/deployment/server-workers/) is a Python Web Server Gateway Interface (WSGI) HTTP server. It is a pre-fork worker model
	*  Gunicorn would act as a **process manager**, listening on the **port** and the **IP**. And it would **transmit** the communication to the worker processes running the **Uvicorn class**.
* [FastAPI](https://nextjs.org/) is a Web framework for developing RESTful APIs in Python.
	* minimalistic, simple and scales well
* [Celery](https://docs.celeryq.dev/) **soon** + optional
* [Flower](https://flower.readthedocs.io/en/latest/) **soon** + optional
* [Redis](https://redis.io/) is an in-memory data structure store, used as a distributed, in-memory key–value database, cache and message broker
* [Motor](https://motor.readthedocs.io/) presents a coroutine-based API for non-blocking access to MongoDB
* [MongoDB](https://svelte.dev/) is a source-available cross-platform document-oriented database program. Classified as a NoSQL database program, MongoDB uses JSON-like documents with optional schemas.
	* **Sharding** is the process of storing data records across multiple machines and it is **MongoDB**'s approach to meeting the demands of data growth.
* [Docker](https://www.docker.com/) **container** is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

Set of instructions to get started with FastyAPI

### Prerequisites

* [Python3](https://www.python.org/downloads/)
* pip3
* venv
	```sh
   python3 -m pip install --user virtualenv
   ```
  
### Environment setup

1. Create the environment
   ```sh
   python3 -m venv .
   ```
2. Activate the environment
   ```sh
   source env/bin/activate
   ```

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/achaayb/FastyAPI
   ```
2. Install the dependencies
   ```sh
   cd FastyAPI 
   pip3 install -r requirements.txt
   ```
 
 ### Running and testing

3. run uvicorn
   ```sh
   uvicorn app:app --reload
   ```
4. test the app
	* navigate to : http://localhost:8000
	* response should be something like this :
		```json
	   {"data":"","code":"success","message":"FastyAPI live!"}
		```

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ROADMAP -->
## Roadmap

- [x] Base boilerplate
- [ ] Follow a naming convention
- [ ] Add comments and stuff
- [ ] Optimise the base boilerplate
- [ ] Finish up the base stack
    - [ ] Gunicorn w/uvicorn workers
    - [ ] FastAPI
    - [ ] Motor
    - [ ] Mongodb (sharding)
- [ ] Stress test 1
	- [ ] Normal test (fork)
	- [ ] Websocket stress (fork)
- [ ] implement stack extentions
	- [ ]  Celery
	- [ ] Redis
	- [ ] Flower
- [ ] Stress test 2
	- [ ] Normal test (fork)
	- [ ] Cpu bound operations test (fork)
- [ ] Docker

See the [open issues](https://github.com/achaayb/FastyAPI/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>

Project Link: [https://github.com/achaayb/FastyAPI](https://github.com/achaayb/FastyAPI)

<p align="right">(<a href="#top">back to top</a>)</p>
