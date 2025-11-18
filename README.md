# Amazon MCP Server

A Model Context Protocol (MCP) server for Amazon services integration.

## Overview

This project implements an MCP server that provides tools and resources for interacting with Amazon services. MCP (Model Context Protocol) is a standardized way to connect AI models with external systems and data sources.

## Features

- **Amazon Services Integration**: Connect to various Amazon Web Services
- **MCP Protocol Compliance**: Implements the Model Context Protocol specification
- **Tool Provision**: Provides tools for AI models to interact with Amazon services
- **Resource Management**: Handles Amazon service resources efficiently

## Prerequisites

- Python 3.8 or higher
- AWS credentials configured (AWS CLI or environment variables)
- Required Python packages (see requirements.txt)

## Installation

1. Clone this repository:
```bash
git clone https://github.com/srivatsa18/My-Projects-Stuff.git
cd My-Projects-Stuff
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Configure AWS credentials:
```bash
aws configure
```

## Usage

Run the MCP server:

```bash
python amazon-mcp-server.py
```

### Configuration

The server can be configured through environment variables:

- `AWS_REGION`: AWS region to use (default: us-east-1)
- `AWS_ACCESS_KEY_ID`: AWS access key ID
- `AWS_SECRET_ACCESS_KEY`: AWS secret access key
- `MCP_SERVER_PORT`: Port to run the MCP server on (default: 8000)

## Supported Amazon Services

- **S3**: Object storage operations
- **EC2**: Instance management
- **Lambda**: Function execution
- **DynamoDB**: Database operations
- **CloudWatch**: Monitoring and logging

## MCP Tools Available

- `list_s3_buckets`: List all S3 buckets
- `get_s3_object`: Retrieve objects from S3
- `list_ec2_instances`: List EC2 instances
- `invoke_lambda_function`: Execute Lambda functions
- `query_dynamodb`: Query DynamoDB tables

## Development

### Project Structure

```
.
├── amazon-mcp-server.py    # Main MCP server implementation
├── README.md              # This file
├── requirements.txt       # Python dependencies
└── tests/                # Test files
```

### Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and commit: `git commit -am 'Add feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

### Testing

Run the test suite:

```bash
python -m pytest tests/
```

## Security Considerations

- Ensure AWS credentials are properly secured
- Use IAM roles with minimal required permissions
- Keep dependencies updated for security patches
- Validate all inputs from MCP clients

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For support and questions:

- Create an issue in this repository
- Check the [MCP documentation](https://modelcontextprotocol.io/)
- Review AWS service documentation

## Changelog

### Version 1.0.0
- Initial MCP server implementation
- Basic Amazon services integration
- Core tool set for S3, EC2, Lambda, DynamoDB, and CloudWatch

## Related Projects

- [Model Context Protocol](https://github.com/modelcontextprotocol)
- [AWS SDK for Python (Boto3)](https://github.com/boto/boto3)
- [MCP Specification](https://spec.modelcontextprotocol.io/)

---

**Note**: This is a development project. Please review and test thoroughly before using in production environments.