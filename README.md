# TOLLIS (Toll Interoperability System)
This project implements an integrated software system for managing the interoperability of toll systems across Greek motorways. The system collects, stores, analyzes, and exposes toll-pass data through a RESTful API, a Command Line Interface (CLI), and a web-based frontend.

It supports core operations such as toll-pass registration, financial settlement calculations between operators, data analysis for stakeholders, and administrative actions (system initialization, data import, health checks).
The CLI mirrors these operations, enabling scripted interaction with the system.
The project also includes complete documentation (SRS, UML diagrams, API specs), automated tests, and use of GitHub project management and AI-assisted development tools.


Software Dependencies :
- Python >= 3.10 (in PATH)
- MySQL >= 8.0
- Web Browser (Chrome,Firefox,Microsoft Edge etc...) with Javascript Enabled.

- ATTENTION! If you want to deploy this project on a mac/linux (generally unix) then use MakefileForMac.Simply delete the main Makefile (it is for windows) and rename MakefileForMac to Makefile.Then proceed normally.

- To install all dependencies,create the database and generate all the needed certificates, use make scratch from the root directory of the project.
We advise against doing that however.It is better to run db_create.sql on your local database connection (localhost:3306) (located in back-end/rest_api/database) and then use make.

```console
foo@bar: softeng24-27 $ make scratch
```

```console
make scratch
```

- To do all of the above without creating the database automatically then simply use make

```console
foo@bar: softeng24-27 $ make
```

```console
make
```

- To run the api use make run_api

```console
foo@bar: softeng24-27 $ make run_api
```

```console
make run_api
```

- To run the Web Portal use make run_portal

```console
foo@bar: softeng24-27 $ make run_portal
```

```console
make run_portal
```

The address at which the API and Portal are available are displayed on the console after they have started running like this:
```console
* Running on https://{your_ip_address}:{port}
```

- To user the cli interface :
```console
foo@bar: softeng24-27 $ cd cli-client
foo@bar: cli-client $ python ./se2427.py {commands}
```

```console
cd cli-client
```

```console
python ./se2427.py {commands}
```
