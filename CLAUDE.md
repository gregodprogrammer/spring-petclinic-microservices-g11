# Spring PetClinic Microservices — G11 Project

## Project Identity
- Project name:    Spring PetClinic Microservices G11
- GitHub username: gregodprogrammer
- GitHub repo:     https://github.com/gregodprogrammer/spring-petclinic-microservices
- Production URL:  https://gregddevops.com.ng
- Group:           G11

## AWS Infrastructure
- Region:          af-south-1 (Africa — Cape Town)
- AWS Account ID:  118821711881
- ECR Registry:    118821711881.dkr.ecr.af-south-1.amazonaws.com
- EKS Cluster:     petclinic-cluster-g11
- K8s Namespace:   petclinic-staging-g11

## Services and Ports
- config-server      → 8888 (starts FIRST)
- discovery-server   → 8761 (starts SECOND)
- api-gateway        → 8080 (public entry point)
- customers-service  → 8081
- vets-service       → 8083
- visits-service     → 8082
- genai-service      → varies

## Run Locally
docker compose up -d
# Wait 3 minutes then open http://localhost:8080
# Stop: docker compose down

## Naming Convention G11
- EKS Cluster:   petclinic-cluster-g11
- K8s Namespace: petclinic-staging-g11
- ECR prefix:    spring-petclinic-g11-*
- Helm release:  petclinic-g11

## Phases
- Phase 1: Install all tools ✅
- Phase 2: AWS setup ✅
- Phase 3: Clone project + CLAUDE.md ← HERE
- Phase 4: Run locally with docker compose
- Phase 5: GitHub repo + CI/CD
- Phase 6: EKS cluster + deploy
- Phase 7: OpenAI GenAI service
- Phase 8: Domain + HTTPS
