# Stage 1: Compile and Build angular codebase

# Use official node image as the base image
FROM node:latest as build

RUN apt-get update \
	&& apt-get install -yq --no-install-recommends \
	nodejs

# Set the working directory
WORKDIR ~/Second_Semester/AMI/Covid19_co2_emission_project-master/Energy-predictor/

# Add the source code to app
COPY ./ ~/Second_Semester/AMI/Covid19_co2_emission_project-master/Energy-predictor/

# Install all the dependencies
RUN npm cache clean
RUN npm install

# Generate the build of the application
RUN npm run build


# Stage 2: Serve app with nginx server

# Use official nginx image as the base image
FROM nginx:latest

# Copy the build output to replace the default nginx contents.
COPY --from=build ~/Second_Semester/AMI/Covid19_co2_emission_project-master/Energy-predictor/ usr/share/nginx/html

# Expose port 80
EXPOSE 80
