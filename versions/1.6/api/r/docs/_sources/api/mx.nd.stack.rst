

``mx.nd.stack``
==============================

Description
----------------------

Join a sequence of arrays along a new axis.
The axis parameter specifies the index of the new axis in the dimensions of the
result. For example, if axis=0 it will be the first dimension and if axis=-1 it
will be the last dimension.

**Example**::

	 x = [1, 2]
	 y = [3, 4]
	 stack(x, y) = [[1, 2],
	 [3, 4]]
	 stack(x, y, axis=1) = [[1, 3],
	 [2, 4]]
	 
	 **Example**::
	 
	 x = [1, 2]
	 y = [3, 4]
	 stack(x, y) = [[1, 2],
	 [3, 4]]
	 stack(x, y, axis=1) = [[1, 3],
	 [2, 4]]
	 
	 
Arguments
------------------

+----------------------------------------+------------------------------------------------------------+
| Argument                               | Description                                                |
+========================================+============================================================+
| ``data``                               | NDArray-or-Symbol[].                                       |
|                                        |                                                            |
|                                        | List of arrays to stack                                    |
+----------------------------------------+------------------------------------------------------------+
| ``axis``                               | int, optional, default='0'.                                |
|                                        |                                                            |
|                                        | The axis in the result array along which the input arrays  |
|                                        | are                                                        |
|                                        | stacked.                                                   |
+----------------------------------------+------------------------------------------------------------+
| ``num.args``                           | int, required.                                             |
|                                        |                                                            |
|                                        | Number of inputs to be stacked.                            |
+----------------------------------------+------------------------------------------------------------+

Value
----------

``out`` The result mx.ndarray


