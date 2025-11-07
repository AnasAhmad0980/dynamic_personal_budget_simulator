git clone https://github.com/AnasAhmad0980/dynamic_personal_budget_simulator.git

1.	Install uv (if not installed already in team mates remote computers)

curl -LsSf https://astral.sh/uv/install.sh | sh


 restart terminal or CMD if necessary

2.	Sync environment and install dependencies

uv sync

3.	Activate venv

source .venv/bin/activate

4.	Create local .env from template and fill real values

cp .env.example .env

Edit .env: 
set SECRET_KEY (generated earlier or generate new), and DB values as needed.


5.	Run migrations & start server

python manage.py migrate

uv run manage.py runserver

