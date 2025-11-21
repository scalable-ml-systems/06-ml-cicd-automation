# 06-ml-cicd-automation
ML CI/CD Automation

``` 
projectX-xxxxx/
│
├── src/                          # All Python source code (training, inference)
│   ├── training/                 # Model training modules
│   ├── inference/                # Serving code (FastAPI, Triton clients, etc.)
│   └── common/                   # Shared utilities (logging, metrics, config)
│
├── infra/                        # Infrastructure-as-Code
│   ├── terraform/                # AWS/GCP/Azure resources
│   ├── kubernetes/               # Manifests, Helm charts
│   └── docker/                   # Additional Dockerfiles (builder, runtime)
│
├── pipelines/                    # Workflow orchestration + CI/CD
│   ├── airflow/                  # DAGs (if applicable)
│   ├── prefect/                  # Flows (if using Prefect)
│   ├── ci/                       # GitHub Actions pipelines
│   └── scripts/                  # Automation scripts (bash, python)
│
├── configs/                      # Configurations for reproducibility
│   ├── training/                 # Training configs (YAML)
│   ├── serving/                  # Inference configs
│   └── system/                   # Environment, paths, variables
│
├── notebooks/                    # Exploratory work
│   ├── exploration/              # Data EDA, prototyping
│   └── experiments/              # Model experiments
│
├── tests/                        # Tests for reliability
│   ├── unit/                     # Unit tests
│   ├── integration/              # Pipeline/model tests
│   └── load/                     # Optional: load & performance tests
│
├── docs/                         # Documentation and architecture
│   ├── architecture/             # System diagrams, flows
│   ├── api/                      # OpenAPI specs, API docs
│   └── READMEs/                  # Additional markdown docs
│
├── scripts/                      # Utility scripts (data prep, setup, etc.)
│
├── Makefile                      # One-line commands: train, test, build, deploy
├── Dockerfile                    # Primary container definition
├── requirements.txt              # Python deps (or pyproject.toml)
├── .gitignore                    # Ignore junk files
├── LICENSE                       # MIT or Apache-2.0
└── README.md                     # Clean, focused project overview

```
