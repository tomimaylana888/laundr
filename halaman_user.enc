<!DOCTYPE html>
<html>
    <head>
            <meta charset="UTF-8">
            <title>Halaman user</title>
            <link rel="stylesheet" href="bootstrap-4.3.1-dist/css/bootstrap.css">
            <style type="text/css">
                 body{
                    background-image:url('123.jpg') ;
                }
            </style>
    </head>
    <body>
          <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
             <a class="navbar-brand" href="halaman_admin.php">Admin</a>
             <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
             </button>
                 <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav mr-auto">
                    <li class="nav-item active">
                          <a class="nav-link" href="halaman_member.php">Member</a>
                        </li>
                        <li class="nav-item active">
                          <a class="nav-link" href="halaman_paket.php">Paket</a>
                        </li>
                        <li class="nav-item active">
                          <a class="nav-link" href="halaman_outlet.php">Outlet</a>
                        </li>
                        <li class="nav-item active">
                          <a class="nav-link" href="halaman_detail_transaksi.php">Detail transaksi</a>
                        </li>
                        <li class="nav-item active">
                          <a class="nav-link" href="halaman_transaksi.php">Transaksi</a>
                        </li>
                          </a>
                      </ul>
                      <form class="form-inline my-2 my-lg-0">
                        <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
                        <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
                     
                      </form>
                    </div>
                  </nav>
                  <div class="wrap">
                        <div class="header">            
                        <center><h1>Halaman User</h1></center>
                    </div> 
                    
                    <?php
                        require "db.php";

                        $db = new Database();
                        $data = $db->getAll('user');

                    ?>
                      <div class="container mt-5">
                     <table class="table">
                        <thead class="thead-dark">
                                <tr>
                                   <th scope="col">id user</th>
                                   <th scope="col">id outlet</th>
                                   <th scope="col">nama</th>
                                   <th scope="col">username</th>
                                   <th scope="col">password</th>
                                   <th scope="col">role</th>
                                   <th scope="col" style="min-width:175px;">Aksi </th>
                                </tr> 
                                
                        </thead>
                        <?php
                          foreach($data as $d):
                        ?>
                            <tr>
                               <th scope="row"><?php echo $d['id_user'];?></th>
                               <td><?php echo $d['id_outlet'];?></td> 
                               <td><?php echo $d['nama'];?></td> 
                               <td><?php echo $d['username'];?></td> 
                               <td><?php echo $d['password'];?></td>
                               <td><?php echo $d['role'];?></td> 
                               <td>
                                 <a href="form_ubah_user.php?id=<?php echo $d['id_user'];?>" class="btn btn-primary">Edit</a>

                                 <a href="proses_hapus_user.php?id=<?php echo $d['id_user'];?>" class="btn btn-danger" onclick="return confirm('Apakah Anda Yakin Akan Menghapus Data Ini?')">Hapus</a>
                                </td>
                          </tr>
                          <?php endforeach; ?>
                     </table>
        </div>
        <center><a href="form_tambah_user.php" class="btn btn-warning">Tambah!</a></center>        
      </body>
</html>
