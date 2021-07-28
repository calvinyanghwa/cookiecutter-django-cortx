# Django + CORTX Cookiecutter

A simple [cookiecutter](https://github.com/cookiecutter/cookiecutter) template that fuses Django and CORTX as the key object storage solution, into one full stack application.

### Motivations

Using Cookiecutter, the community is able to automatically spin up a Django project that is integrated with CORTX and has prebuilt file upload functionalities.

With Django as one of the top Python-based web frameworks, cookiecutter templates are able to lower the barrier of entry for integrating with CORTX as the object storage solution of choice. We also hope that future solutions will be able to leverage on this cookiecutter template when they want to integrate CORTX with their Django project.

## Installation

1. Install cookiecutter and cookiecutter-django-cortx:

```
pip install cookiecutter
cd <your-working-directory>
cookiecutter <url> # TODO
```

2. Install development requirements:

```
pip install -r requirements/local.txt
```

3. Set environment variables for CORTX (**IMPORTANT**):

In `.env` found in the root file, fill in `ACCESS_KEY_ID`, `SECRET_ACCESS_KEY`, `BUCKET_NAME` and `CORTX_ENDPOINT_URL` with your own values.

4. Apply migrations:

```
python manage.py migrate
```

5. Create a new admin user:

```
python manage.py createsuperuser
```

6. Run the server:

```
python manage.py runserver
```

Navigate to `127.0.0.1:8000/admin` to access the file upload functionality. Then, feel free to build further on top of the cookiecutter project.

## Contributors

This project was submitted for Seagate CORTX Integration Challenge: Singapore.

- Calvin Yang
- Denise Lee
- Lee Yu Jing
- Mitra Hadesh
- Teo Zhi Wei

## TODOs

- Add more functionality into the File Upload API.
- Make it look prettier on the admin interface.
- Update the URL in the README above.
