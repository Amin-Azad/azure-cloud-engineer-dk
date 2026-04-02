# Day 1 — Azure CLI + Linux Foundations

## Azure CLI Commands

Authentication:
az login

Check active subscription:
az account show --output table

List subscriptions:
az account list --output table

List resource groups:
az group list --output table

List locations (filtered):
az account list-locations --output table | grep -i europe

Create resource group:
az group create --name myRG --location northeurope

Show resource group:
az group show --name myRG

Delete resource group:
az group delete --name myRG --yes

----------------------------------------

## Linux Fundamentals

Navigation:
pwd
ls
ls -la
cd ~
cd ..

File & Folder Operations:
mkdir folder
mkdir -p path
touch file.txt
rm -rf folder

File Viewing:
cat file.txt
less file.txt

Searching:
grep -i europe file.txt

----------------------------------------

## Important Concepts

Command Options:
-l = short option
--output = full option

Pipe:
|
Pass output from one command to another

Example:
az account list-locations | grep europe

AND / OR:
&& = run next command if previous succeeds
| (in grep) = OR condition

Example:
grep -E "sweden|norway"

----------------------------------------

## Key Learnings

- Azure CLI manages cloud resources from terminal
- Resource groups are the main working unit
- Linux terminal is the primary interface for engineers
- Always verify location using pwd before deleting
