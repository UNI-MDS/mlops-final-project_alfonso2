# MLOps Introduction: Final Project
FInal work description in  the [final_project_description.md](final_project_description.md) file.

Student info:
- Full name:
- e-mail:
- Grupo: 

## Project Name: [Insert Your Project Title Here]

Put here the description, implementation doc, info, results, etc about your work.
You can also use links/reference to other documents/files form this repository or outside resources.

Remarks: feel free to modify this file for documentation 
TODO:
...


### Serving

a.a.a.a

### Predictions
Running predictions using `curl` command:
```sh
curl -X POST http://127.0.0.1:5000/predict2 -H "Content-Type: application/json" -d '{"experience_score": 4, "test_score": 7, "interview_score": 8}
```

Using Python request library: 
```sh
python src/predict.py
```