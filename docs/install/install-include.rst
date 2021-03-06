Select your preferences and run the install command.

.. role:: title
.. role:: opt
   :class: option
.. role:: act
   :class: active option

.. container:: install

  .. container:: opt-group

     :title:`OS:`
     :opt:`Linux`
     :opt:`macOS`
     :opt:`Windows`

  .. container:: opt-group

     :title:`Version:`
     :act:`Stable`
     :opt:`Nightly`
     :opt:`Source`

     .. raw:: html

        <div class="mdl-tooltip" data-mdl-for="stable">Stable Release.</div>
        <div class="mdl-tooltip" data-mdl-for="nightly">Nightly build with latest features.</div>
        <div class="mdl-tooltip" data-mdl-for="source">Install GluonCV from source.</div>


  .. container:: opt-group

     :title:`Backend:`
     :act:`Native`
     :opt:`CUDA`
     :opt:`MKL-DNN`
     :opt:`CUDA + MKL-DNN`

     .. raw:: html

        <div class="mdl-tooltip" data-mdl-for="native">Build-in backend for CPU.</div>
        <div class="mdl-tooltip" data-mdl-for="cuda">Required to run on Nvidia GPUs.</div>
        <div class="mdl-tooltip" data-mdl-for="mkl-dnn">Accelerate Intel CPU performance.</div>
        <div class="mdl-tooltip" data-mdl-for="cuda-mkl-dnn">Enable both Nvidia CPUs and Inter CPU acceleration.</div>

  .. admonition:: Prerequisites:

     - Requires `pip >= 9. <https://pip.pypa.io/en/stable/installing/>`_.
       Both Python 2 and Python 3 are supported.

     .. container:: nightly

        - Nightly build provides latest features for enthusiasts.

  .. admonition:: Command:

     .. container:: stable

        .. container:: native

           .. code-block:: bash

              pip install --upgrade mxnet gluoncv

        .. container:: cuda

           .. code-block:: bash

              # Here we assume CUDA 10.0 is installed. You can change the number
              # according to your own CUDA version.
              pip install --upgrade mxnet-cu100 gluoncv

        .. container:: mkl-dnn

           .. code-block:: bash

              pip install --upgrade mxnet-mkl gluoncv

        .. container:: cuda-mkl-dnn

           .. code-block:: bash

              # Here we assume CUDA 10.0 is installed. You can change the number
              # according to your own CUDA version.
              pip install --upgrade mxnet-cu100mkl gluoncv

     .. container:: nightly

        .. container:: native

           .. code-block:: bash

              pip install --pre --upgrade mxnet gluoncv

        .. container:: cuda

           .. code-block:: bash

              pip install --pre --upgrade mxnet-cu100 gluoncv

        .. container:: mkl-dnn

           .. code-block:: bash

              pip install --pre --upgrade mxnet-mkl gluoncv

        .. container:: cuda-mkl-dnn

           .. code-block:: bash

               pip install --pre --upgrade mxnet-cu100mkl gluoncv

     .. container:: source

        .. container:: native

           .. code-block:: bash

              pip install --pre --upgrade mxnet
              git clone https://github.com/dmlc/gluon-cv
              cd gluon-cv && python setup.py install --user

        .. container:: cuda

           .. code-block:: bash

              pip install --pre --upgrade mxnet-cu100
              git clone https://github.com/dmlc/gluon-cv
              cd gluon-cv && python setup.py install --user

        .. container:: mkl-dnn

           .. code-block:: bash

              pip install --pre --upgrade mxnet-mkl
              git clone https://github.com/dmlc/gluon-cv
              cd gluon-cv && python setup.py install --user

        .. container:: cuda-mkl-dnn

           .. code-block:: bash

               pip install --pre --upgrade mxnet-cu100mkl
               git clone https://github.com/dmlc/gluon-cv
               cd gluon-cv && python setup.py install --user
