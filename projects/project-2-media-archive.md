# Enterprise Media Archive

## Executive overview

I designed and implemented a serverless media archive adopted by a leading African podcast network, supporting over 10 TB of media workloads.

## Business challenge

Large media files called for reliable transfers and long-term retention, with distinct permissions for uploaders and administrators.

## Solution architecture

A web interface uses Cognito for authentication and API Gateway and Lambda for upload coordination. Media files travel directly from the browser to Amazon S3.

## Technical implementation

The archive uses presigned URLs and multipart uploads. Parallel part transfers, retrying individual parts and handling interrupted uploads were design considerations. The web interface supports file management.

## Personal responsibilities

I designed and implemented the archive, including its ingestion, access and storage lifecycle architecture.

## Security and governance

The design uses encryption and least-privilege IAM. Uploader and administrator roles scope file operations, and CloudWatch supports operational visibility.

## Cost optimisation

The lifecycle strategy moves eligible objects to archival tiers. S3 storage is chargeable, and tier selection needs to account for request and retrieval costs.

## Project outcomes

The archive was implemented and used by the media production team. Measured transfer performance and realised savings are unverified.

## Architecture diagram

![Enterprise Media Archive architecture](../diagrams/project-2-architecture.svg)

[Editable Graphviz source](../diagrams/project-2-architecture.dot)

## Technologies used

Amazon S3, AWS Lambda, Amazon API Gateway, Amazon Cognito, AWS IAM and Amazon CloudWatch.

## Lessons learned

Separate upload coordination from file transfer and plan recovery at the part level for large uploads.
