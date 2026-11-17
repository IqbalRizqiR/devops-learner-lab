FROM public.ecr.aws/lambda/python:3.11

# Install Python dependencies
RUN pip install --no-cache-dir \
    psycopg2-binary \
    boto3

# Copy application codess
COPY app.py ${LAMBDA_TASK_ROOT}/

# Set the handler
CMD ["app.lambda_handler"]