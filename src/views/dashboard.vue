<template>
  <div class="dashboard">
    <div class="row">
      <div class="col-lg-6">
        <div class="panel panel-default">
          <div class="panel-heading">
            <h3 class="panel-title">Billboard <small class="pull-right"><a href="http://www.billboard.com/charts/hot-100" target="_blank">{{$t('more')}}</a></small></h3>
          </div>
          <div class="panel-body">
            <table class="table table-hover table-striped table-bordered">
              <thead>
                <tr>
                  <th>{{$t('rank')}}</th>
                  <th>{{$t('songName')}}</th>
                </tr>
              </thead>
              <tbody>
                <tr v-for="(item, index) in billboardList">
                  <td>{{index + 1}}</td>
                  <td>{{item}}</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
      <div class="col-lg-6">
        <div class="panel panel-default">
          <div class="panel-heading">
            <h3 class="panel-title">IMDb <small class="pull-right"><a href="http://www.imdb.com/chart/top?ref_=nv_wl_img_3" target="_blank">{{$t('more')}}</a></small></h3>
          </div>
          <div class="panel-body">
            <table class="table table-hover table-striped table-bordered">
              <thead>
                <tr>
                  <th>{{$t('rank')}}</th>
                  <th>{{$t('filmName')}}</th>
                </tr>
              </thead>
              <tbody>
                <tr v-for="(item, index) in imdblist">
                  <td>{{index+1}}</td>
                  <td>{{item}}</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>
<script>
  export default {
    data() {
      return {
        billboardList: ['Closer', 'StarBoy', 'Heathens', 'Let Me Love You', 'Broccoli', '24K Magic', 'Side To Side', 'Cold Water', 'Juju On That Beat (TZ Anthem)', 'I Hate U I Love U' ],
        imdblist: ['The Shawshank Redemption', 'The Godfather', 'The Godfather: Part II ', 'The Dark Knight ', '12 Angry Men', ' Schindler\'s List', 'Pulp Fiction', 'The Lord of the Rings: The Return of the King', ' The Good, the Bad and the Ugly', ' Fight Club']
      }
    },
    locales: {
      ch: { more: '更多', rank:'排行', songName: '歌名', 'filmName': '电影名' },
      en: { more: 'More', rank:'Rank', songName: 'Song name', 'filmName': 'Film name' }
    }
  }
</script>
<style>
  .dashboard .table{
    margin-bottom: 0;
  }
</style>
