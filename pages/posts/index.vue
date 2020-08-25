<template>
  <div>
    <p class="text-white font-extrabold text-3xl md:text-5xl">
						POSTS
					</p>
    <div class="flex flex-wrap justify-between pt-12 -mx-6">
      	<div v-for="(post,index) in posts" :key=" `__post_$(index)`" :class="`w-full md:w-${ post.tail } p-6 flex flex-col flex-grow flex-shrink`">
            <PostPreview

              :id           = "post.id"
              :title        = "post.title"
              :description  = "post.description"
              :thumbnail    = "post.thumbnail"
              :userImage    = "post.userImage"
              :timeToRead   = "post.timeToRead"
              :tail         = "post.tail"
              >

            </PostPreview>
        </div>
		</div>
  </div>
</template>
<script>
  import PostPreview from '~/components/PostPreview.vue'

  export default {
    components: {
          PostPreview
    },
    data(){
          return {

              posts : [
                  { tail:'1/3',id: '1', title:'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',description:'lorem ipsum', thumbnail:'https://source.unsplash.com/collection/225/800x600',userImage:'http://i.pravatar.cc/300',timeToRead :'1 MIN READ' },
                  { tail:'1/3',id: '2', title:'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',description:'lorem ipsum', thumbnail:'https://source.unsplash.com/collection/3106804/800x600',userImage:'http://i.pravatar.cc/300',timeToRead :'1 MIN READ' },
                  { tail:'1/3',id: '3', title:'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',description:'lorem ipsum', thumbnail:'https://source.unsplash.com/collection/3657445/800x600',userImage:'http://i.pravatar.cc/300',timeToRead :'1 MIN READ' },
                  { tail:'1/2',id: '4', title:'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',description:'lorem ipsum', thumbnail:'https://source.unsplash.com/collection/764827/800x600',userImage:'http://i.pravatar.cc/300',timeToRead :'1 MIN READ' },
                  { tail:'1/2',id: '5', title:'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',description:'lorem ipsum', thumbnail:'https://source.unsplash.com/collection/1118905/800x600',userImage:'http://i.pravatar.cc/300',timeToRead :'1 MIN READ' },
                  { tail:'1/3',id: '6', title:'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',description:'lorem ipsum', thumbnail:'https://source.unsplash.com/collection/325867/800x600',userImage:'http://i.pravatar.cc/300',timeToRead :'1 MIN READ' },
                  { tail:'1/3',id: '7', title:'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',description:'lorem ipsum', thumbnail:'https://source.unsplash.com/collection/1118905/800x600',userImage:'http://i.pravatar.cc/300',timeToRead :'1 MIN READ' },
                  { tail:'1/3',id: '8', title:'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',description:'lorem ipsum', thumbnail:'https://source.unsplash.com/collection/325867/800x600',userImage:'http://i.pravatar.cc/300',timeToRead :'1 MIN READ' },
]

        }
      }
  }
</script>
