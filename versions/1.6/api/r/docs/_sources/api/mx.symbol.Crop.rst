

``mx.symbol.Crop``
====================================

Description
----------------------


.. note:: `Crop` is deprecated. Use `slice` instead.

Crop the 2nd and 3rd dim of input data, with the corresponding size of h_w or
with width and height of the second input symbol, i.e., with one input, we need h_w to
specify the crop height and width, otherwise the second input symbol's size will be used



Usage
----------

.. code:: r

	mx.symbol.Crop(...)

Arguments
------------------

+----------------------------------------+------------------------------------------------------------+
| Argument                               | Description                                                |
+========================================+============================================================+
| ``data``                               | Symbol or Symbol[].                                        |
|                                        |                                                            |
|                                        | Tensor or List of Tensors, the second input will be used   |
|                                        | as crop_like shape                                         |
|                                        | reference                                                  |
+----------------------------------------+------------------------------------------------------------+
| ``num.args``                           | int, required.                                             |
|                                        |                                                            |
|                                        | Number of inputs for crop, if equals one, then we will use |
|                                        | the h_wfor crop height and width, else if equals two, then |
|                                        | we will use the heightand width of the second input        |
|                                        | symbol, we name crop_like                                  |
|                                        | here                                                       |
+----------------------------------------+------------------------------------------------------------+
| ``offset``                             | Shape(tuple), optional, default=[0,0].                     |
|                                        |                                                            |
|                                        | crop offset coordinate: (y, x)                             |
+----------------------------------------+------------------------------------------------------------+
| ``h.w``                                | Shape(tuple), optional, default=[0,0].                     |
|                                        |                                                            |
|                                        | crop height and width: (h, w)                              |
+----------------------------------------+------------------------------------------------------------+
| ``center.crop``                        | boolean, optional, default=0.                              |
|                                        |                                                            |
|                                        | If set to true, then it will use be the center_crop,or it  |
|                                        | will crop using the shape of                               |
|                                        | crop_like                                                  |
+----------------------------------------+------------------------------------------------------------+
| ``name``                               | string, optional.                                          |
|                                        |                                                            |
|                                        | Name of the resulting symbol.                              |
+----------------------------------------+------------------------------------------------------------+

Value
----------

``out`` The result mx.symbol


Link to Source Code: http://github.com/apache/incubator-mxnet/blob/1.6.0/src/operator/crop.cc#L50

