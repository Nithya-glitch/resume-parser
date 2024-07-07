# resume-parser
To share the solution via GitHub, you can create a repository and upload a Python script or Jupyter notebook that utilizes a pre-trained language model (like GPT-4) to parse the resume text into the desired JSON format. 
import json

resume_text = """
nithya sree s
no.18/6 gandhimathi street vetri nagar extension
chennai,tamil nadu,600082
Email: ns4103@srmist.edu.in
Phone: 7395910319

Education:
- Bachelor of Science in Computer Science
  SRNM INSTITUTE OF SCIENCE AND TECHNOLOGY
  Graduated: june 2025

Work Experience:

                "title": "Software Developer Intern and data analyst intern",
                "company": "AICTE",
                "dates": "dec-2023",
                "responsibilities": [
                    "Developed and maintained web applications using python and sql",
                    "Collaborated with a team to design and implement new features."

Skills:
            "programming_languages": ["Python", "Java", "C++",sql,matlab,uipath ,uipath automation,r language,linux],
            "web_development": ["HTML", "CSS", "JavaScript", "React"],
            "tools": ["Git", "Docker", "Kubernetes"]

Projects:  
                "name": "AI Chatbot for alumni engagement",
                "description": "Developed a chatbot using Python and NLP techniques to assist with customer service inquiries." 
                "name": "drowsiness detection in traffic signals(reading eyes of the driver)
                "description": "Developed a Machiene learning concept using CNN architecture."",
            


Certifications:{
                "name": "design pattern",
                "issuer": "university of alberta", 
                "name": "i/o pscychology"
                "issuer": "coursera",
                "name":"matlab"
                "issuer":"MATLAB ON RAMP"
                "name":"advanced excel"
                "issuer":"SRMIST" 
                "name":"sql/plsql"
                "issuer":"oracle academey"
                "name":"data analytics"
                 "issuer":"accenture"
                 "name":"data mining with python"
                 "issuer":"infosys"
            
                
            }
        ]
    }


# Placeholder function to simulate parsing
def parse_resume_to_json(resume_text):
    return {
        "personal_information": {
            "name": "NITHYA SREE S",
            "address": "NO,18/5 ,gandhimathi street vetri nagar extension ,chennai-600082,India",
            "email": "ns4103@srmist.edu.in",
            "phone": "7395910319"
        },
        "education": [
            {
                "degree": "Bachelor of Science in Computer Science with business system",
                "institution": "SRM institute of science and technology",
                "graduation_date": "june 2025"
            }
        ],
        "work_experience": [
            {
                "title": "Software Developer Intern and data analyst intern",
                "company": "AICTE",
                "dates": "dec-2023",
                "responsibilities": [
                    "Developed and maintained web applications using python and sql",
                    "Collaborated with a team to design and implement new features."
                ]
            }
        ],
        "skills": {
            "programming_languages": ["Python", "Java", "C++",sql,matlab,uipath ,uipath automation,r language,linux],
            "web_development": ["HTML", "CSS", "JavaScript", "React"],
            "tools": ["Git", "Docker", "Kubernetes"]
        },
        "projects": [
            {
                "name": "AI Chatbot for alumni engagement",
                "description": "Developed a chatbot using Python and NLP techniques to assist with customer service inquiries." 
                "name": "drowsiness detection in traffic signals(reading eyes of the driver)
                "description": "Developed a Machiene learning concept using CNN architecture."",
            }
        ],
        "certifications": [
            {
                "name": "design pattern",
                "issuer": "university of alberta", 
                "name": "i/o pscychology"
                "issuer": "coursera",
                "name":"matlab"
                "issuer":"MATLAB ON RAMP"
                "name":"advanced excel"
                "issuer":"SRMIST" 
                "name":"sql/plsql"
                "issuer":"oracle academey"
                "name":"data analytics"
                 "issuer":"accenture"
                 "name":"data mining with python"
                 "issuer":"infosys"
            
                
            }
        ]
    }

# Convert resume text to JSON
resume_json = parse_resume_to_json(resume_text)

# Print JSON output
print(json.dumps(resume_json, indent=2))

