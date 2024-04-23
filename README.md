# `DB` [AI Processor][https://github.com/app-generator/ai-processor]  

Simple tool that extracts information from an SQLite source using human language queries. The stack uses a NextJs frontend and a Django (API) for users management and OpenAI interface.  

<br />

> Download Sources: private repository, for access contact [AppSeed](https://appseed.us/) 

```bash
$ git clone https://github.com/app-generator/priv-ai-processor.git
$ cd priv-ai-processor 
```

<br />

> **Django** Backend

Edit `backend-Django/.env` and add you own `OpenAI API KEY`. 

```bash
$ cd backend-Django                # change DIR to the backend code 
$ virtualenv env                   # create a new virtual environment  
$ source env/bin/activate          # activate the VENV
$ pip install -r requirements.txt  # install modules 
$ python manage.py makemigrations  # migrate DB
$ python manage.py migrate         # apply DB changes 
$ python manage.py runserver       # Start the development Server 
```

The backend starts on Django's default address: `http://localhost:8000`

<br />

> **NextJS** UI 

```bash
$ cd frontend-Nextjs                # change DIR to the frontend code  
$ npm install -g next               # Install NextJs globally
$ npm i                             # install dependencies
$ npm run dev                       # Start the development Next Server
```

<br />

## How to use the tool

> Create a new user or authenticate using the default one:

- **user**     : `test`
- **email**    : `test@appseed.us`
- **password** : `pass`

> Add your own OPEN API Key 

Access the settings page and save your OpenAI API key 

> Upload a new SQLite file 

Navigate to the SQLite Uploads file and add a new file. Once uploaded, we can query start quering the database. 

> Query the information using OpenAI console

Here are some query samples: 

- `List all tables registered in the database`
- `List all products starting with the cheapest`

Once another SQLite file is uploaded, we can query other specific questions. 

<br />

## License

[@EULA](https://github.com/app-generator/license-eula)

<br />

---
`DB` [AI Processor][https://github.com/app-generator/ai-processor] - AI/ML Starter provideed **[AppSeed](https://appseed.us)**.
