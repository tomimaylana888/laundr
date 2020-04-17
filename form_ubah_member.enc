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
            $member = $db->getById('member', ['id_member'=>$id]);

            foreach($member as $m):
                ?>

        <div class="card bg-secondary text-light">
                <div class="card-header">
                    <h2>Form ubah member</h2>
                </div>
                <div class="card-body">
                    <form action="proses_ubah_member.php" method="POST">
                <div class="form-group">
                    <label class="label-control">ID Member</label> 
                    <input class="form-control" type="number" name="id_member" placeholder="id_member"  value="<?php echo $m['id_member'];?>" readonly>
                </div>
                <div class="form-group">
                    <label class="label-control">Nama </label> 
                    <input class="form-control" type="text" name="nama" placeholder="Nama" value="<?php echo $m['nama'];?>" required>
                </div>
                <div class="form-group">
                    <label class="label-control">Alamat</label> 
                    <input class="form-control" type="text" name="alamat" placeholder="alamat" value="<?php echo $m['alamat'];?>" required>
                </div>
                <div class="form-group">
                    <label class="label-control">Jenis Kelamin</label>
                    <br>
                    <select name="jenis_kelamin" class="form-control"> 
                        <option > L </option>
                        <option > P </option>
                    </select>
                </div>
                <div class="Form-group" >
                    <label class="label-control">Tlp</label> 
                    <input class="form-control" type="text" name="tlp" placeholder="Tlp" value="<?php echo $m['tlp'];?>" required>
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