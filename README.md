# 👋 Hi, I'm Evan! 

```python
# Initialize main profile configurations
import pytorch as torch
import pandas as pd
from pyspark.sql import SparkSession

class Engineer:
    def __init__(self):
        self.name = "Evan Diewald"
        self.role = "Data & ML Engineer"
        self.location = "Cleveland, OH"
        self.company = "Amazon Web Services (AWS)"
        
    def get_socials(self) -> pd.DataFrame:
        return pd.DataFrame({
            "platform": ["LinkedIn", "Medium", "Google Scholar"],
            "url": [
                "linkedin.com/in/evan-diewald-68786413b/",
                "evandiewald.medium.com/",
                "scholar.google.com/citations?hl=en&user=PqHDYuYAAAAJ&view_op=list_works",
            ]
        })

    def get_tech_stack(self) -> torch.Tensor:
        return torch.stack([
            "PyTorch", "TensorFlow", "huggingface",   # ML & Deep Learning
            "Python", "SQL", "TypeScript",            # Languages
            "Spark", "Airflow", "dbt",                # Data Engineering
            "Terraform", "Docker", "AWS CDK",         # Infrastructure
        ])
        
# Initialize Spark session for education history
spark = SparkSession.builder.appName("education").getOrCreate()

education = spark.createDataFrame([
    ("Carnegie Mellon University", "Master's in Mechanical Engineering", "2019-2021"),
    ("Penn State University", "Bachelor's in Mechanical Engineering", "2016-2019")
], ["institution", "degree", "years"])

# Function to get current focus areas
def current_focus() -> list:
    return [
        "Large Language Models 🤖",
        "MLOps & Model Deployment 🚀",
        "Infrastructure as Code ⚡",
        "Data Pipeline Optimization 📊"
    ]

if you.are_interested_in(["GenAI", "Data Engineering", "AWS"]):
    feel_free_to.connect()
```
