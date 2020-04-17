<!DOCTYPE html>
    <html>
        <head>
            <meta charset="UTF-8">
            <title>Form Ubah Outlet</title>
            <link rel="stylesheet" href="bootstrap-4.3.1-dist/css/bootstrap.css">
            <style type="text/css">
                 body{
                    background-image:url('gray.jpg') ;
                }
            </style>
        </head>
        <body class="container mt-5">
        <?php

            require 'db.php';

            $id=$_GET['id'];

            $db = new Database();
            $outlet = $db->getById('outlet', ['id_outlet'=>$id]);

            foreach($outlet as $o):
                ?>

        <div class="card bg-secondary text-light">
                <div class="card-header">
                    <h2>Form ubah Outlet</h2>
                </div>
                <div class="card-body">
                    <form action="ubah_outlet.php" method="POST">
                <div class="form-group">
                <div class="form-group">
                    <label class="label-control">ID Outlet</label> 
                    <input class="form-control" type="number" name="id_outlet" placeholder="id_outlet"  value="<?php echo $o['id_outlet'];?>" readonly>
                </div>
                    <label class="label-control">Nama </label> 
                    <input class="form-control" type="text" name="nama" placeholder="Nama" value="<?php echo $o['nama'];?>" required>
                </div>
                <div class="form-group">
                    <label class="label-control">Alamat</label> 
                    <input class="form-control" type="text" name="alamat" placeholder="alamat"value="<?php echo $o['alamat'];?>" required>
                </div>
                <div class="Form-group" >
                    <label class="label-control">Tlp</label> 
                    <input class="form-control" type="text" name="tlp" placeholder="Tlp" value="<?php echo $o['tlp'];?>" required>
                </div>
               <br>
                <button class="btn btn-warning" type="submit">Ubah</button>   
            </form>
        </div>
        </div>
        </div>
        <?php endforeach; ?>
        </body>
</html>