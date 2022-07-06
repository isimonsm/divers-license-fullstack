# divers-license-fullstack
This repository is a skeleton for implementing the divers license task for a Full Stack Developer.

## Frontend
The frontend application is initialized using `create-react-app`. The implementation can be made directly in the `App.js` component.

## Backend
The backend folder contains the data files needed for the task. The rest of the backend implementation (including choice of framework) is up to the interviewee.
The only restriction is that python has to be used.

The data folder contains two csv files that represent the same dataset in two different representations.

The `pixels.csv` is already processed to contain three values in every row:
1. velocity in m/s (attribute used to color the pixels, not normalized to a scale)
2. pixel index x (index of pixel in x-direction)
3. pixel index y (index of pixel in y-direction)

This representation makes it easier to paint on a 2D canvas in the frontend.

The `pointcloud.csv` holds the original data, where the x- and y-values are not normalized to a fixed grid, but rather as a position on a cartesian grid. Parsing this pointcloud progressively is harder and requires the knowledge of the range of x- and y-values in the frontend.

