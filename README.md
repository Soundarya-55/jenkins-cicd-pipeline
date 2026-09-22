# jenkins-cicd-pipeline
<img width="934" height="440" alt="image" src="https://github.com/user-attachments/assets/d99a620e-5998-419b-8e0d-f1791008837d" />

## Steps
                  Developer
                     │
                     │ git push
                     ▼
              ┌─────────────┐
              │   GitHub    │
              │ Repository  │
              └──────┬──────┘
                     │
                  Webhook
                     │
                     ▼
              ┌─────────────┐
              │   Jenkins   │
              └──────┬──────┘
                     │
          ┌──────────┴──────────┐
          │                     │
          ▼                     ▼
     Checkout Code           Build
          │                     │
          └──────────┬──────────┘
                     ▼
                   Test
                     │
                     ▼
              Docker Build
                     │
                     ▼
              Docker Deploy
                     │
                     ▼
             Running Container
                     │
                     ▼
                Application

