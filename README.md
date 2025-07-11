here's how you can add the **"Using Docker Compose"** section with the `docker compose up -d` command to your `README.md`:


## Using Docker Compose

to start the entire app with all services running in the background, use:

```bash
docker compose up -d
````

this will:

* build the images if they don’t exist
* start the frontend, backend, and mongodb containers
* run everything in detached mode (so your terminal stays clean)

to check if all containers are up:

```bash
docker compose ps
```

to see logs from all services:

```bash
docker compose logs -f
```

to stop everything:

```bash
docker compose down
```

Related Blog Post

i wrote a blog documenting everything that went wrong during this project — from mongo crashing to backend errors, weird docker behavior, and how i fixed it all step-by-step.
if you're new to dockerizing a mern stack or just want to avoid the mistakes i made, check it out here:

👉 [**rookie mistakes i made while dockerizing my mern app (and how i fixed them)**](https://mycloudclimb.hashnode.dev/rookie-mistakes-i-made-while-dockerizing-my-mern-app-and-how-i-fixed-them)

it includes fixes, lessons learned, and tips .
