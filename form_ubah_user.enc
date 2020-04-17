<!DOCTYPE html>
    <html>
        <head>
            <meta charset="UTF-8">
            <title>Form Ubah user</title>
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
            $user = $db->getById('user', ['id_user'=>$id]);

            foreach($user as $u):
                ?>

        <div class="card bg-secondary text-light">
                <div class="card-header">
                    <h2>Form ubah User</h2>
                </div>
                <div class="card-body">
                    <form action="proses_ubah_user.php" method="POST">
                <div class="form-group">
                    <label class="label-control">ID User</label> 
                    <input class="form-control" type="number" name="id_user" placeholder="Id User"  value="<?php echo $u['id_user'];?>" readonly>
                </div>
                <div class="form=group">
                    <label class="bmd-label-floating">Id Outlet</label>
                    <select name="id_outlet" class="form-control">
                    <?php 
                    $outlet = $db->getAll('outlet');

                        foreach($outlet as $o):

                    ?>
                        <option value="<?php echo $o['id_outlet']; ?>" class="form-control"><?php echo $o['nama'];?></option>
                        <?php endforeach; ?>
                    </select>
                </div>
                <div class="form-group">
                    <label class="label-control">Nama </label> 
                    <input class="form-control" type="text" name="nama" placeholder="Nama" value="<?php echo $u['nama'];?>" required>
                </div>
                <div class="form-group">
                    <label class="label-control">Username</label> 
                    <input class="form-control" type="text" name="username" placeholder="Username" value="<?php echo $u['username'];?>" required>
                </div>
                <div class="form-group">
                    <label class="label-control">Password</label> 
                    <input class="form-control" type="password" name="password" placeholder="Password"  value="<?php echo $u['password'];?>" readonly>
                </div>
                <div class="form-group">
                <label class="bmd-label-floating">Role</label>
                    <select name="role" class="form-control">
                        <option class="form-control" value="1">Admin</option>
                        <option class="form-control" value="2">Kasir</option>
                        <option class="form-control" value="3">Owner</option>
                    </select>
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