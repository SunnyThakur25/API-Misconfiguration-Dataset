# API-Misconfiguration-Dataset


Overview

This dataset catalogs common API misconfiguration vulnerabilities across various API types, including REST, GraphQL, SOAP, gRPC, WebSocket, and others. Each entry details a specific security issue, its associated risks, impacts, and recommended mitigations, serving as a valuable resource for security researchers, developers, and pentesters.

Dataset Structure

The dataset is stored in API_MISCONFIGURATION_DATASET.jsonl, with each line representing a JSON object for a single vulnerability. The fields for each entry are:





id: Unique identifier (e.g., "api-001")



title: Short description of the issue (e.g., "Verbose Error Messages")



issue: Detailed explanation of the vulnerability



endpoint: Affected API endpoint (e.g., "POST /api/login")



risk: Type of security risk (e.g., "Information Disclosure")



impact: Potential consequences of the vulnerability



recommendation: Suggested mitigation steps



category: Vulnerability category (e.g., "Verbose Errors")



api_type: Type of API affected (e.g., "REST", "GraphQL")

Usage

This dataset can be used for:





Security Training: Educate developers on common API vulnerabilities and best practices.



Penetration Testing: Guide testers in identifying and exploiting misconfigurations.



Automated Scanning: Integrate into tools to detect misconfigurations in API deployments.



Research: Analyze trends in API vulnerabilities across different API types.

Example Entry

{
  "id": "api-001",
  "title": "Verbose Error Messages",
  "issue": "Exposes internal stack trace and system paths in error response.",
  "endpoint": "POST /api/login",
  "risk": "Information Disclosure",
  "impact": "Attacker can gather sensitive environment details for targeted attacks.",
  "recommendation": "Use generic error messages in production and log full details internally.",
  "category": "Verbose Errors",
  "api_type": "REST"
}

Categories

Key vulnerability categories include:





Access Control



Authentication



Verbose Errors



Overly Permissive CORS



Rate Limiting & Abuse



Mass Assignment



Excessive Data Exposure



Insecure Defaults

API Types

The dataset covers:





REST



GraphQL



SOAP



gRPC



WebSocket



Partner APIs



Composite APIs



Public APIs



Internal APIs



Private APIs



JSON-RPC



Open APIs

Contributing

To contribute new vulnerabilities or corrections:





Fork the repository.



Add or modify entries in API_MISCONFIGURATION_DATASET.jsonl.



Ensure each entry follows the defined structure.



Submit a pull request with a clear description of changes.

License

This dataset is licensed under the MIT License. See LICENSE for details.
