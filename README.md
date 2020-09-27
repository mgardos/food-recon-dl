# food-recon-dl

Under model path a sample food prediction model generated with the available notebook is provided in parts. In order to reconstruct the original compressed model file, use the following command:

```
cat food.model.best.hdf5.tar.gz.part0* > food.model.best.hdf5.tar.gz
```

Then, to unpack the model, use the following command:

```
untar -xvf food.model.best.hdf5.tar.gz
```

The resulting hdf5 file can be loaded with Keras API or DL4J API in order to perform predictions.
