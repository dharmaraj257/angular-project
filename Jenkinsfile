#!/bin/bash
echo "${GIT_BRANCH}"
BFRANCH_NAME=${GIT_BRANCH}
echo"BRANCH_NAME"
npm install || exit 1

if ["BRANCH_NAME" == "origin/main"]
then
echo"building development..."
ng build|| exit 1

if ["BRANCH_NAME" == "origin/main"]
then
echo"building staging..."
ng serve| exit 1


