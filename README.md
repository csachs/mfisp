# mfisp

microfluidic image stack processing

Some miscellaneous tools helpful for working with image stacks (with microfluidic structures). Currently contains two utilities:

## Tools

### register

Registration routine from [molyso](https://github.com/modsim/molyso), will automatically register the input stack and possible additional channels.

```bash
> python3 -m mfisp.register --output result.tif --channel 0 input.tif
```

### autorotate

Automatic rotation detection and de-rotation from [molyso](https://github.com/modsim/molyso).
(Hint: Try to have OpenCV installed for your Python version, otherwise the rotation will be *very* slow.
Windows users take a look [here](http://www.lfd.uci.edu/~gohlke/pythonlibs/#opencv).)

```bash
> python3 -m mfisp.autorotate --output result.tif --channel 0 input.tif
```

## License

2-clause BSD.