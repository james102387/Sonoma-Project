## Installation

After downloading the project folder, simple open it in a localhost environment. For quick set up, make sure python 3 is installed on your local machine, navigate to the project root directory and run the following command:

```bash
python -m http.server 8000
```

## Notes

As far as scalability is concerned, if the json source file were to grow substantially, there could be some lag in the time required to retrieve the json data as well as memory buildup from the image storage on the front end. Ideally in this situation we would solve these problems by processing the data server side so that we do not receive large json data sets. This can be accomplished with server side (ajax) processing via datatables js and only loading thumbnail images when they are needed via ajax. In this case, we store the image urls in a global array (but not actually rendering them until their respective product is clicked) since the json data is not a very large set and we are already getting the json data.
