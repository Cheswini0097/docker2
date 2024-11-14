# Build stage
FROM python:3.11-slim-buster AS builder
WORKDIR /app
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
COPY . .
RUN python setup.py bdist_wheel

# Production stage
FROM nginx:latest
COPY --from=builder /app/dist /usr/share/nginx/html
EXPOSE 80