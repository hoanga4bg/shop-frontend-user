<template>
    <div class="technology-wrap">
        <div class="title-posts">
            <h1 class="title-primary"></h1>
            <h1 class="title-sub">NGHIÊN CỨU - CÔNG NGHỆ - TỰ CÔNG BỐ - KIỂM ĐỊNH</h1>
        </div>
        <div class="posts">
            <div class="posts-left">
                <TechnologyItem :dataPosts="dataPosts[0]" />
            </div>
            <div class="posts-right">
                <div class="posts-right-top">
                    <TechnologyItem :dataPosts="dataPosts[1]" />
                </div>
                <div class="posts-right-bottom">
                    <TechnologyItem :dataPosts="dataPosts[2]" />
                </div>
            </div>
        </div>
        <div class="image-post-list">
            <div class="image-zoom" v-viewer>
                <img src="@/assets/Slide_banner-1-1.jpg" alt />
            </div>
            <div class="image-zoom" v-viewer>
                <img src="@/assets/Slide_banner-2.jpg" alt />
            </div>
        </div>
    </div>
</template>
<script>
import TechnologyItem from '@/components/technology/TechnologyItem.vue';
export default {
    name: 'TechnologyPosts',
    components: {
        TechnologyItem
    },
    data() {
        return {
            dataPosts: [
                {
                    title: 'kiểm định chất lượng sản phẩm',
                    content: 'Đầu tiên Đông trùng hạ thảo nên là sản phẩm hoang dã tự nhiên. Đông trùng hạ thảo Hymalya tốt vì được khai thác trên đỉnh núi cao với độ thanh khí tốt. Có 2 vị trí được coi là hàng tốt nhất về xuất xứ là: Nugu Tây Tạng & Thung lũng Dolpa của Nepal.',
                    image: '@/assets/vstp-1.jpg'
                },
                {
                    title: 'Nghiên cứu và phát triển sản phẩm',
                    content: 'Đầu tiên Đông trùng hạ thảo nên là sản phẩm hoang dã tự nhiên. Đông trùng hạ thảo Hymalya tốt vì được khai thác trên đỉnh núi cao với độ thanh khí tốt. ',
                    image: '@/assets/vstp-1.jpg'
                },
                {
                    title: 'Công nghệ sản xuất',
                    content: 'Đầu tiên Đông trùng hạ thảo nên là sản phẩm hoang dã tự nhiên. Đông trùng hạ thảo Hymalya tốt vì được khai thác trên đỉnh núi cao với độ thanh khí tốt. ',
                    image: '@/assets/vstp-1.jpg'
                },
                {
                    title: 'Chứng nhận',
                    content: 'Đầu tiên Đông trùng hạ thảo nên là sản phẩm hoang dã tự nhiên. Đông trùng hạ thảo Hymalya tốt vì được khai thác trên đỉnh núi cao với độ thanh khí tốt. ',
                    image: '@/assets/vstp-1.jpg'
                },
                {
                    title: 'Tự công bố',
                    content: 'Đầu tiên Đông trùng hạ thảo nên là sản phẩm hoang dã tự nhiên. Đông trùng hạ thảo Hymalya tốt vì được khai thác trên đỉnh núi cao với độ thanh khí tốt. ',
                    image: '@/assets/vstp-1.jpg'
                },
            ]
        }
    },
    methods:{

    }
}
</script>

<style scoped>
.technology-wrap {
    padding: 20px 0px;
    background-color: rgb(1, 64, 35);
}

.title-posts {
    width: 60%;
    margin: 0 auto;
}

.title-primary,
.title-sub {
    font-size: 28px;
    color: rgb(242, 160, 41);
}

.posts {
    display: flex;
    margin: 0 auto;
    flex-wrap: wrap;
    justify-content: center;
}

.posts-left {
    width: 500px;
    margin: 10px;
    height: 350px;
}

.posts-right {
    width: 400px;
    margin: 5px;
    height: 350px;
}

.posts-right-top {
    height: calc(50% - 10px);
    margin: 5px 0px 15px 0px;
}

.posts-right-bottom {
    height: calc(50% - 5px);
}

.posts-sub {
    display: flex;
    margin: 0 auto;
    flex-wrap: wrap;
    justify-content: flex-start;
}

.posts-sub-item {
    width: 400px;
    margin: 5px;
    height: 350px;
    height: 175px;
}

.image-zoom {
    height: 200px;
    width: 450px;
    margin: 5px 5px;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    border-radius: 10px;
    cursor: pointer;
    
}
.image-zoom img{
    flex-shrink: 0;
    min-width: 100%;
    min-height: 100%
}

.image-post-list {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

@media only screen and (max-width: 947px) {

    .posts-left{
        height: 165px;
    }
    .posts-right {
        width: 500px;
    }
    .image-zoom{
        width: 500px;
    }
}


@media only screen and (max-width: 785px) {

}
</style>
