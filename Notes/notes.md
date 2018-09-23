- Tensors are similar to NumPy’s ndarrays, with the addition being that Tensors can also be used on a GPU to accelerate computing.
- Any operation that mutates a tensor in-place is post-fixed with an _. For example: `x.copy_(y), x.t_(), will change x`
- The Torch Tensor and NumPy array will share their underlying memory locations, and changing one will change the other.
- Generally, when you have to deal with image, text, audio or video data, you can use standard python packages that load data into  a numpy array. Then you can convert this array into a torch.*Tensor.
    - For images, packages such as Pillow, OpenCV are useful
    - For audio, packages such as scipy and librosa
    - For text, either raw Python or Cython based loading, or NLTK and SpaCy are useful

