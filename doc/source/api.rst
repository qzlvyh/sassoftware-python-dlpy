
.. Copyright SAS Institute

.. currentmodule:: dl_api
.. _api:

*************
API Reference
*************

.. _api.functions:


Applications
------------

.. currentmodule:: dl_api.applications

.. autosummary::
   :toctree: generated/

   LeNet5
   LeNet5_bn
   VGG11
   VGG11_bn
   VGG13
   VGG13_bn
   VGG16
   VGG16_bn
   VGG19
   VGG19_bn
   ResNet18_SAS
   ResNet18_Caffe
   ResNet34_SAS
   ResNet34_Caffe
   ResNet50_SAS
   ResNet50_Caffe
   ResNet101_SAS
   ResNet101_Caffe
   ResNet152_SAS
   ResNet152_Caffe
   wide_resnet
   

ImageTable
----------

The :class:`ImageTable` class is a specialized version of :class:`swat.CASTable`
that includes extra methods for working with images.

.. currentmodule:: dl_api.images

Constructors
~~~~~~~~~~~~

.. autosummary::
   :toctree: generated/

   ImageTable
   ImageTable.from_table
   ImageTable.load_files


Saving
~~~~~~

.. autosummary::
   :toctree: generated/

   ImageTable.to_files
   ImageTable.to_sashdat


Utilities
~~~~~~~~~

.. autosummary::
   :toctree: generated/

   ImageTable.copy_table
   ImageTable.show


Image Processing
~~~~~~~~~~~~~~~~

.. autosummary::
   :toctree: generated/

   ImageTable.crop
   ImageTable.resize
   ImageTable.as_patches
   ImageTable.as_random_patches


Layers
------

.. currentmodule:: dl_api.layers

.. autosummary::
   :toctree: generated/

   Layer
   Layer.summary
   Layer.to_model_params
   InputLayer
   Conv2d
   Pooling
   Dense
   Recurrent
   BN
   Res
   Proj
   OutputLayer


Models
------

.. currentmodule:: dl_api.model

.. autosummary::
   :toctree: generated/

   Model
   Model.from_table
   Model.from_sashdat
   Model.load
   Model.set_weights
   Model.load_weights
   Model.load_weights_from_CAFFE
   Model.load_weights_from_table
   Model.set_weights_attr
   Model.load_weights_attr
   Model.model_info
   Model.fit
   Model.tune
   Model.plot_training_history
   Model.predict
   Model.plot_predict_res
   Model.get_feature_maps
   Model.get_features
   Model.heat_map_analysis
   Model.plot_heat_map
   Model.save_to_astore
   Model.save_to_table
   Model.deploy
   Model.count_params
   Model.summary
   Model.plot_network


Feature Maps
------------

.. currentmodule:: dl_api.model

.. autosummary::
   :toctree: generated/

   FeatureMaps
   FeatureMaps.display


Functions
---------

.. currentmodule:: dl_api.model

.. autosummary::
   :toctree: generated/

   get_num_configs
   get_str_configs
   extract_input_layer
   extract_conv_layer
   extract_pooling_layer
   extract_batchnorm_layer
   extract_residual_layer
   extract_fc_layer
   extract_output_layer
   layer_to_node
   layer_to_edge
   model_to_graph


Residual Networks
-----------------

.. currentmodule:: dl_api.ResNet

.. autosummary::
   :toctree: generated/

   Block

.. autosummary::
   :toctree: generated/

   ResBlock
   ResBlock.compile

.. autosummary::
   :toctree: generated/

   ResBlockBN
   ResBlockBN.compile

.. autosummary::
   :toctree: generated/

   ResBlock_Caffe
   ResBlock_Caffe.compile


RNN Model
---------

.. currentmodule:: dl_api.RNN

.. autosummary::
   :toctree: generated/

   RNN
   RNN.add
   RNN.pop
   RNN.switch
   RNN.compile
   RNN.summary
   RNN.plot_network

.. autosummary::
   :toctree: generated/

   layer_to_node
   layer_to_edge
   model_to_graph


Sequential Model
----------------

.. currentmodule:: dl_api.Sequential

.. autosummary::
   :toctree: generated/

   Sequential
   Sequential.add
   Sequential.pop
   Sequential.switch
   Sequential.compile


Splitting Utilities
-------------------

.. currentmodule:: dl_api.splitting

.. autosummary::
   :toctree: generated/

   two_way_split
   three_way_split
   