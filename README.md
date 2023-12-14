# Feel-and-Think

# Writing the sequence diagram in Mermaid syntax
mermaid_diagram = """
sequenceDiagram
    participant User
    participant S3
    participant Lambda
    participant EC2

    User->>S3: Uploads data
    S3->>Lambda: Triggers on data upload
    Lambda->>EC2: Starts EC2 instance
    EC2->>S3: Processes and returns data
    User->>S3: Accesses processed data
"""

mermaid_diagram

