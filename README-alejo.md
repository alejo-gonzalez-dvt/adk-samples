https://github.com/google/adk-samples/tree/main/agents/customer-service

# Virtual Env Creation
<!-- python -m venv .venv -->

# Virtual Env Activation: 
.venv\Scripts\Activate.ps1

# Go into agent
cd agents/customer-service

pip install google-adk
pip install poetry
poetry install
poetry env activate

$env:GOOGLE_CLOUD_PROJECT = "alejo-gonzalez-sandbox-02"
$env:GOOGLE_GENAI_USE_VERTEXAI = "1"
$env:GOOGLE_CLOUD_LOCATION = "us-central1"

adk web