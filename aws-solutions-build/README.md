# To create the image
```docker build -t aws-solutions-build .```

# To run the container and start in an interactive bash
```docker run -it aws-solutions-build /bin/bash```

# To run the container, copy the current working diretory to a folder on the container called work-dir, and start in an interactive bash
```docker run -it -v $(pwd):/work-dir aws-solutions-build /bin/bash```

# Or if on windows: 
```docker run -it -v %cd%:/work-dir aws-solutions-build /bin/bash```

# Once there
cd work-dir/deployment
chmod +x build-s3-dist.sh
./build-s3-dish.sh solution-bucket solution-prefix solution-version