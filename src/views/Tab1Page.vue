<template>
    <ion-page>
      <ion-header :translucent="true">
        <ion-toolbar>
          <ion-title class="home">Home</ion-title>
        </ion-toolbar>
      </ion-header>
      
      <ion-content :fullscreen="true">
        <ion-grid>
            <ion-row>
                <ion-column>
                    <ion-card class="kiri">
                        <ion-card-subtitle>Kolam</ion-card-subtitle>
                        <ion-card-title>10</ion-card-title>
                    </ion-card>
                </ion-column>>
                <ion-column>
                    <ion-card class="kanan">
                        <ion-card-subtitle>Kolam Aktif</ion-card-subtitle>
                        <ion-card-title>8</ion-card-title>
                    </ion-card>
                </ion-column>>
            </ion-row>>
            <ion-row>
                <ion-column>
                    <ion-card class="kiri">
                        <ion-card-subtitle>Ikan Hidup</ion-card-subtitle>
                        <ion-card-title>182 <span class="tambahan">ekor</span></ion-card-title>
                    </ion-card>
                </ion-column>>
                <ion-column>
                    <ion-card class="kanan">
                        <ion-card-subtitle>Ikan Mati</ion-card-subtitle>
                        <ion-card-title>89 <span class="tambahan">ekor</span></ion-card-title>
                    </ion-card>
                </ion-column>>
            </ion-row>>
            <ion-row>
                <ion-column>
                    <ion-card class="kiri">
                        <ion-card-subtitle>Panen 2022</ion-card-subtitle>
                        <ion-card-title>109 <span class="tambahan">kg</span></ion-card-title>
                    </ion-card>
                </ion-column>>
                <ion-column>
                    <ion-card class="kanan">
                        <ion-card-subtitle>Total Pakan</ion-card-subtitle>
                        <ion-card-title>223 <span class="tambahan">kg</span></ion-card-title>
                    </ion-card>
                </ion-column>>
            </ion-row>>
        </ion-grid>>
        <ion-header :translucent="true">
            <ion-toolbar>
                <ion-title class="menu">Total Berat Ikan</ion-title>
            </ion-toolbar>
        </ion-header>>
        <ion-slides>
          <ion-slide>
            <ion-grid>
              <ion-row>
                <ion-column>
                  <ion-card class="ikan">
                    <img class="picture" src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBxMSEhUTExEVFhUVEhUSFRUVFRUSGBUVFRcWFxUSFRYYHSggGBolGxUVITEhJSkrLi4uFx8zODMsNygtLisBCgoKDg0OGhAQGismHR4tLS0rLS0rLS0tKy4tLTEtKy0tLS0tKy0tLS0tLS0tLS0rLS0tLSsrLS0tLSstNS0tLf/AABEIAOEA4QMBIgACEQEDEQH/xAAbAAEAAQUBAAAAAAAAAAAAAAAAAQIEBQYHA//EADgQAAIBAgIIAwYFBAMBAAAAAAABAgMRBCEFBhIxQVFhgSIycRNSkaGxwRRCYtHwByNy4TOi0hX/xAAZAQEAAwEBAAAAAAAAAAAAAAAAAQMEAgX/xAAjEQEBAAMAAgICAgMAAAAAAAAAAQIDESExBBJBUVJhIjJC/9oADAMBAAIRAxEAPwDtAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAARKQEOQgiIx/m8rAAAAAAAAAAAAAAABEpARKQgiIx5/wAZWAAAAAAAAAAAAAAAAAI2f515kgAAAAAAAAAAAAAAAAARskgAAAAAAAACmUioAAAAAAAAAAAAAAAAACmUioAAAAAAAAAAAAAAAAAAAAAAAAFM5AS5ElMYkt23gSRKSSbbSSV23kkubZZYzS9Ckm51Y87J7Tfokc81k1hqYp7MbxpJ5Q58nPm+m5fMt16ss7/TjLORs+ldd6FNuNNe0a/Nuj2e+X06mu4jXmvLdsxXRfds1xYST4D/AOfLq+xsx04Y/hTc8qztPW+vxn8br6MyOH1zqR8y2vR/aX7mnywbXM85qXX4k3Xjfwj7V1TR2tlGpZS8L9H9DP06ikrxaa5rM4ZCrJGc0TrJWovKXZ5p9CnP40/5d47f26yDB6C1mpYi0W9ip7jeUv8AB8fTeZwyZY3G8q6WX0AFM5WISmUrElEY8WVgAAAMTpvT9LDLxO8uEU+PX9t5iNatbo0b06T2qm5tbo9/59zmuIxMqktqTcm97+y5I06tHfOSrPZzxG21tcq1SacMrNc0vgsvjc6XJHH9C005QjxlOMcvE82lw3HYGyPkYyckNdt6gAGdaAAAAY7Sml4UcnnL3f3JktvIi3i/qTSV27Lm9yMRjNO0obryfTJGtaR0zOq83lyWSMVOq2acPj/yVZbf02DF6z1ZeW0V03mHxGkJzd5TlLuyzBoxwxnqKrlaVKuZ5OykpLJSytyYqkS8jfKUX8ztC7R6JHltHpGWRCRq55TwkZcEXBFwMfV0UuDLGvo+UebXTMz+2LodONWSa3G36v661KaUK6dSK3TuttLk/e7/ABLSvhYS3rusmYyvo6zus/k/9kZY45TlJbPTq+j9KUa8dqlUjK29J5x/yjvRdKJxNVKlKSlFuLW5xbi13TNr0Jr3UjaOIj7Re/FRjNeq8svl3Mufx7P9V2O2X26IC10dpGlXjtUpqS48HHpKLzRdGezi0NR141kdBewpP+5JeJr8kXuiv1P5L1RsGmtJRw1GdaW6KyXvSeUY939zi+MxUqs5Tk7ynJylLq+XL7F+jX9r2+or2Zc8PObu883xPXD0lfNX6HkmllcusKk3vXfd9czazts1LoOpWjktmmtt25rKKy6tfA6IYTVPRvsaKb89S0nla0fyx+bfczZ5+7L7ZeGnCcgACp2AFvj8ZGjB1J7l8W3uSJk6MZrFpn2K2Iedq9/dT4+ppNWu27t3b4lWOxjqzlN75Sb9FwXZWXYtzfr1zGMuWXari1m5y2YRhOpOW/ZhTi5zduL2YswWr2tNPGTq040HScIe1g/aOptw24wammlaXji8st6txM5CVnuTycWmrqUZJxlGS4pptNdS0wGjaFBSVChGnttOTTnNu25Xm21FclkTlMvtOXwmXHl77XIB5VahY4UzlmKkv7c+rivmeaRXWWUFxlLafov9AXkUSUKR5V8VGPmaRAuNopr1VBXk7fX+ephcRpzhBW6mLq15Sd22/TMJbPhcYqjaXDuXRreiJbFRN7mtl993zSNkQE2IJuQB5VKae9XLKto5PysyDRDRKGMw0quHmqkG4yW6S3W5Pg10Z1PVzTCxVJTyU14ZxXCS4r9L3r4cDn5TGKWayeeayeeT3FW3XM5/brDO4qv6h6b9vVjSg/7VJt3We3U3OXoldJ9Zc0apGBksfh/E2mkv50LdUuvyv9f2LMcZjORFvb15UqSvufa/1RuGp2gPa1duaXsqbTfHalvjD04vsuJi9C6KlWnGMc23bNuy5yfRK7Oq6OwMKFONOCtGK9LvjJ9WU79n1nJ7rvXj29XIAMLQAAAYzWPB+1w81neKdSNle8oReVuN02u5kwTLy9RZ1yRVf0/9kyVPp80ZvWfVyVKUqlKLdJ3k0s3T4tW93rw48zWto9LHKZTsZbLLyrzaRDmi09oRtHfEPepW5Hje5Qe9KFwhXQpXfJb2+SW9lEfFJz4bo+glNy8Ed35nz6HtbK3IhK10hKex4N987b7Z7vkYOWGm82m/mbIyhoDXfwzX5WUypvr8zYnBFEqKfL4AYBK3B/M2HR+M245+ZZPryZ4SwcfdX0JoUFB3StdWAv8A2vUj8QWzkUMngu3ikebxfQttlmS0ZoCviEnCHhf55eGPLJvf2uRbJ5pO1ZvFExrM2/A6iRWdWs3+mmrf9pXv8EbBgtA4al5aMb2teXjee/OV7dijL5GE9eVk1ZVyqvK+8sJS5fQ2PXXQ7w1S8f8AiqK8OOy15oP0yt0fQ1lX3rLn+5djlMp2K7LLyth1V0n7KpGazzzW5Si8mjqtGqpxUou6aumcQw9TZlfc+ayv6/7Oi6p6V3Qk/DPyvlLl3/Yo36+z7RZry54baADE0AAAAAAaprBqiqjdShaMt7p7oy6xf5X03ehtYOsM7jexFxl9uO4jDzpycJwcZLepKz9eq6nmkddx2Ap1o7NWCkuF966xazXY1jG6k53o1MvdqfaSX1Xc2YfIxvvwouqz01ClRvm8kt7Z51q1/DC9uL5mR0jobEQb9pSkoLjHxR9XKN0u5YxSW4vll9K74TRWyipzKWUsCvaIczzuNokVuoQmUxDYEtlLZVSpyk9mMXKT3RinJv0SNi0dqhWqWdS1KP6vFLtFbu7Rzlnjj7pMbfTWz1xeGqU1eVKpFNXTlTnGNvVqx0vRegKFCzjHan78/FLtwj2Mpcz5fK8+Itmr9uF1q8nut33fI3D+n2s0Yv8AC1WoqUr0m3kpS30m+F3mura4o3PHaBw1a7nQptv8yioy+KzZrekf6f03nRqOL92eafez+hF3YZzl8EwyxvY3UFvo6nONKEaktqcYpSl7zXH13FwZF7G6xaKWKoTpbpeaD5TXlfpvT6NnGpwcJOMk04tp801k0+p3c5//AFF0A0/xdKN1l7ZLhwVVdNyfZ8zT8fZy/WqtmPfLS7rJ9n+5mNEYi0lF9v2MHB3L3DLNJdLG1Q65ojH+0ppt+KPhl/67r7l7A1LVbE2qK+6a2X/ks0/qu5t55u3H65NWF7AAFboAAAAAAAALXE6Oo1PPShJ83FX+O8ugJeDA4zVLDzT2YypyadpRlKST4PZk2muhzfSWHr0Kjp1MpR6XUlwlF8UzsxjtN6FpYqGzUWa8k15ot8ua5p5F+vfcb/l6V565fTkH4uX6fmvuUrH9F8f9Ga0tqTiqTezH2sOEqfm7wed/S5hZ6Drp50p94uLNkzxvqqLjY9Fjei+Zsmp88LVn7KvB+0b8DcpKEv0WTVny5/C+r/gKi3xfdfdFeHykrPZkmmnyazUl1TQyn2nOk8V2rDYWFNWpwjBcopR+Nt56nhgK7qUqc2rOdOM2uTlFNr5nuebWuAAIAAAAAAIlFNWaumrNPNNPg0SAOY64apSoN1qEW6OblFZypdVzh9OPM1nDVc953Q07WPUWFVuphmqVR5uD/wCOb7eR+mXTia9W/wDGSnPX+Yx2g6/lknulF/NM6EzmOjsLUpSVOpCVOpdRSdmpZ2vFrJ+qOns5+RzsqdSAAZloAAKXIqAAAAAAAAAAE3IAB5lvPAUm7ulTvz2I3+Ni4A6CQAAplIqAAAAAAAAAAAAAAAAAAAAAAAABTKQEuRJRGPErAAAAAAAAAAAAAAABTKVgJcrElEY8WVgAAAAAAAAAAAAAAAARJlKjcrAAAAAAAAAAAAAAAAAESZSo3KwAAAAAAAAAAAAAAAAAAAAAAAAAFyGhFASAAAAAAAAAAAAAAAAEw0RFASAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAD//2Q==" alt="">
                    <h1 class="textIkan">Ikan <br> <span class="berat">200kg</span></h1>
                  </ion-card>
                </ion-column>
                <ion-column>
                  <ion-card class="ikan">
                    <img class="picture" src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBxMSEhUTExEVFhUVEhUSFRUVFRUSGBUVFRcWFxUSFRYYHSggGBolGxUVITEhJSkrLi4uFx8zODMsNygtLisBCgoKDg0OGhAQGismHR4tLS0rLS0rLS0tKy4tLTEtKy0tLS0tKy0tLS0tLS0tLS0rLS0tLSsrLS0tLSstNS0tLf/AABEIAOEA4QMBIgACEQEDEQH/xAAbAAEAAQUBAAAAAAAAAAAAAAAAAQIEBQYHA//EADgQAAIBAgIIAwYFBAMBAAAAAAABAgMRBCEFBhIxQVFhgSIycRNSkaGxwRRCYtHwByNy4TOi0hX/xAAZAQEAAwEBAAAAAAAAAAAAAAAAAQMEAgX/xAAjEQEBAAMAAgICAgMAAAAAAAAAAQIDESExBBJBUVJhIjJC/9oADAMBAAIRAxEAPwDtAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAARKQEOQgiIx/m8rAAAAAAAAAAAAAAABEpARKQgiIx5/wAZWAAAAAAAAAAAAAAAAAI2f515kgAAAAAAAAAAAAAAAAARskgAAAAAAAACmUioAAAAAAAAAAAAAAAAACmUioAAAAAAAAAAAAAAAAAAAAAAAAFM5AS5ElMYkt23gSRKSSbbSSV23kkubZZYzS9Ckm51Y87J7Tfokc81k1hqYp7MbxpJ5Q58nPm+m5fMt16ss7/TjLORs+ldd6FNuNNe0a/Nuj2e+X06mu4jXmvLdsxXRfds1xYST4D/AOfLq+xsx04Y/hTc8qztPW+vxn8br6MyOH1zqR8y2vR/aX7mnywbXM85qXX4k3Xjfwj7V1TR2tlGpZS8L9H9DP06ikrxaa5rM4ZCrJGc0TrJWovKXZ5p9CnP40/5d47f26yDB6C1mpYi0W9ip7jeUv8AB8fTeZwyZY3G8q6WX0AFM5WISmUrElEY8WVgAAAMTpvT9LDLxO8uEU+PX9t5iNatbo0b06T2qm5tbo9/59zmuIxMqktqTcm97+y5I06tHfOSrPZzxG21tcq1SacMrNc0vgsvjc6XJHH9C005QjxlOMcvE82lw3HYGyPkYyckNdt6gAGdaAAAAY7Sml4UcnnL3f3JktvIi3i/qTSV27Lm9yMRjNO0obryfTJGtaR0zOq83lyWSMVOq2acPj/yVZbf02DF6z1ZeW0V03mHxGkJzd5TlLuyzBoxwxnqKrlaVKuZ5OykpLJSytyYqkS8jfKUX8ztC7R6JHltHpGWRCRq55TwkZcEXBFwMfV0UuDLGvo+UebXTMz+2LodONWSa3G36v661KaUK6dSK3TuttLk/e7/ABLSvhYS3rusmYyvo6zus/k/9kZY45TlJbPTq+j9KUa8dqlUjK29J5x/yjvRdKJxNVKlKSlFuLW5xbi13TNr0Jr3UjaOIj7Re/FRjNeq8svl3Mufx7P9V2O2X26IC10dpGlXjtUpqS48HHpKLzRdGezi0NR141kdBewpP+5JeJr8kXuiv1P5L1RsGmtJRw1GdaW6KyXvSeUY939zi+MxUqs5Tk7ynJylLq+XL7F+jX9r2+or2Zc8PObu883xPXD0lfNX6HkmllcusKk3vXfd9czazts1LoOpWjktmmtt25rKKy6tfA6IYTVPRvsaKb89S0nla0fyx+bfczZ5+7L7ZeGnCcgACp2AFvj8ZGjB1J7l8W3uSJk6MZrFpn2K2Iedq9/dT4+ppNWu27t3b4lWOxjqzlN75Sb9FwXZWXYtzfr1zGMuWXari1m5y2YRhOpOW/ZhTi5zduL2YswWr2tNPGTq040HScIe1g/aOptw24wammlaXji8st6txM5CVnuTycWmrqUZJxlGS4pptNdS0wGjaFBSVChGnttOTTnNu25Xm21FclkTlMvtOXwmXHl77XIB5VahY4UzlmKkv7c+rivmeaRXWWUFxlLafov9AXkUSUKR5V8VGPmaRAuNopr1VBXk7fX+ephcRpzhBW6mLq15Sd22/TMJbPhcYqjaXDuXRreiJbFRN7mtl993zSNkQE2IJuQB5VKae9XLKto5PysyDRDRKGMw0quHmqkG4yW6S3W5Pg10Z1PVzTCxVJTyU14ZxXCS4r9L3r4cDn5TGKWayeeayeeT3FW3XM5/brDO4qv6h6b9vVjSg/7VJt3We3U3OXoldJ9Zc0apGBksfh/E2mkv50LdUuvyv9f2LMcZjORFvb15UqSvufa/1RuGp2gPa1duaXsqbTfHalvjD04vsuJi9C6KlWnGMc23bNuy5yfRK7Oq6OwMKFONOCtGK9LvjJ9WU79n1nJ7rvXj29XIAMLQAAAYzWPB+1w81neKdSNle8oReVuN02u5kwTLy9RZ1yRVf0/9kyVPp80ZvWfVyVKUqlKLdJ3k0s3T4tW93rw48zWto9LHKZTsZbLLyrzaRDmi09oRtHfEPepW5Hje5Qe9KFwhXQpXfJb2+SW9lEfFJz4bo+glNy8Ed35nz6HtbK3IhK10hKex4N987b7Z7vkYOWGm82m/mbIyhoDXfwzX5WUypvr8zYnBFEqKfL4AYBK3B/M2HR+M245+ZZPryZ4SwcfdX0JoUFB3StdWAv8A2vUj8QWzkUMngu3ikebxfQttlmS0ZoCviEnCHhf55eGPLJvf2uRbJ5pO1ZvFExrM2/A6iRWdWs3+mmrf9pXv8EbBgtA4al5aMb2teXjee/OV7dijL5GE9eVk1ZVyqvK+8sJS5fQ2PXXQ7w1S8f8AiqK8OOy15oP0yt0fQ1lX3rLn+5djlMp2K7LLyth1V0n7KpGazzzW5Si8mjqtGqpxUou6aumcQw9TZlfc+ayv6/7Oi6p6V3Qk/DPyvlLl3/Yo36+z7RZry54baADE0AAAAAAaprBqiqjdShaMt7p7oy6xf5X03ehtYOsM7jexFxl9uO4jDzpycJwcZLepKz9eq6nmkddx2Ap1o7NWCkuF966xazXY1jG6k53o1MvdqfaSX1Xc2YfIxvvwouqz01ClRvm8kt7Z51q1/DC9uL5mR0jobEQb9pSkoLjHxR9XKN0u5YxSW4vll9K74TRWyipzKWUsCvaIczzuNokVuoQmUxDYEtlLZVSpyk9mMXKT3RinJv0SNi0dqhWqWdS1KP6vFLtFbu7Rzlnjj7pMbfTWz1xeGqU1eVKpFNXTlTnGNvVqx0vRegKFCzjHan78/FLtwj2Mpcz5fK8+Itmr9uF1q8nut33fI3D+n2s0Yv8AC1WoqUr0m3kpS30m+F3mura4o3PHaBw1a7nQptv8yioy+KzZrekf6f03nRqOL92eafez+hF3YZzl8EwyxvY3UFvo6nONKEaktqcYpSl7zXH13FwZF7G6xaKWKoTpbpeaD5TXlfpvT6NnGpwcJOMk04tp801k0+p3c5//AFF0A0/xdKN1l7ZLhwVVdNyfZ8zT8fZy/WqtmPfLS7rJ9n+5mNEYi0lF9v2MHB3L3DLNJdLG1Q65ojH+0ppt+KPhl/67r7l7A1LVbE2qK+6a2X/ks0/qu5t55u3H65NWF7AAFboAAAAAAAALXE6Oo1PPShJ83FX+O8ugJeDA4zVLDzT2YypyadpRlKST4PZk2muhzfSWHr0Kjp1MpR6XUlwlF8UzsxjtN6FpYqGzUWa8k15ot8ua5p5F+vfcb/l6V565fTkH4uX6fmvuUrH9F8f9Ga0tqTiqTezH2sOEqfm7wed/S5hZ6Drp50p94uLNkzxvqqLjY9Fjei+Zsmp88LVn7KvB+0b8DcpKEv0WTVny5/C+r/gKi3xfdfdFeHykrPZkmmnyazUl1TQyn2nOk8V2rDYWFNWpwjBcopR+Nt56nhgK7qUqc2rOdOM2uTlFNr5nuebWuAAIAAAAAAIlFNWaumrNPNNPg0SAOY64apSoN1qEW6OblFZypdVzh9OPM1nDVc953Q07WPUWFVuphmqVR5uD/wCOb7eR+mXTia9W/wDGSnPX+Yx2g6/lknulF/NM6EzmOjsLUpSVOpCVOpdRSdmpZ2vFrJ+qOns5+RzsqdSAAZloAAKXIqAAAAAAAAAAE3IAB5lvPAUm7ulTvz2I3+Ni4A6CQAAplIqAAAAAAAAAAAAAAAAAAAAAAAABTKQEuRJRGPErAAAAAAAAAAAAAAABTKVgJcrElEY8WVgAAAAAAAAAAAAAAAARJlKjcrAAAAAAAAAAAAAAAAAESZSo3KwAAAAAAAAAAAAAAAAAAAAAAAAAFyGhFASAAAAAAAAAAAAAAAAEw0RFASAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAD//2Q==" alt="">
                    <h1 class="textIkan">Ikan <br> <span class="berat">200kg</span></h1>
                  </ion-card>
                </ion-column>
              </ion-row>
            </ion-grid>
          </ion-slide>
          <ion-slide>
            <ion-grid>
              <ion-row>
                <ion-column>
                  <ion-card class="ikan">
                    <img class="picture" src="data:image/jpeg;base64,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" alt="">
                    <h1 class="textIkan">Ikan <br> <span class="berat">200kg</span></h1>
                  </ion-card>
                </ion-column>
                <ion-column>
                  <ion-card class="ikan">
                    <img class="picture" src="data:image/jpeg;base64,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" alt="">
                    <h1 class="textIkan">Ikan <br> <span class="berat">200kg</span></h1>
                  </ion-card>
                </ion-column>
              </ion-row>
            </ion-grid>
          </ion-slide>
        </ion-slides>
        <ion-header :translucent="true">
            <ion-toolbar>
                <ion-title class="menu2">Kualitas air</ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-slides>
          <ion-slide>
            <ion-grid>
              <ion-row>
                <ion-column>
                  <ion-card class="kualitas">
                    <h1 class="text"><span class="ktitle">Ph</span><br><span class="kopsi">Normal: </span><span class="khasil">6 kolam </span><br><span class="kopsi">Abnormal: </span><span class="khasil">6 kolam</span> </h1>
                  </ion-card>
                </ion-column>
                <ion-column>
                  <ion-card class="kualitas">
                    <h1 class="text"><span class="ktitle">DO</span><br><span class="kopsi">Normal: </span><span class="khasil">6 kg </span><br><span class="kopsi">Abnormal: </span><span class="khasil">6 kg</span> </h1>
                  </ion-card>
                </ion-column>
              </ion-row>
            </ion-grid>
          </ion-slide>
          <ion-slide>
            <ion-grid>
              <ion-row>
                <ion-column>
                  <ion-card class="kualitas">
                    <h1 class="textIkan">Ikan <br> <span class="berat">200kg</span></h1>
                  </ion-card>
                </ion-column>
                <ion-column>
                  <ion-card class="kualitas">
                    <h1 class="textIkan">Ikan <br> <span class="berat">200kg</span></h1>
                  </ion-card>
                </ion-column>
              </ion-row>
            </ion-grid>
          </ion-slide>
        </ion-slides>
      </ion-content>
    </ion-page>
  </template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';

export default  defineComponent({
  name: 'Tab1Page',
  components: { IonHeader, IonToolbar, IonTitle, IonContent, IonPage }
});
</script>
  <style scoped>
  ion-title.home{
    color:white;
    margin-bottom: 0px;
  }
  ion-title.menu{
    margin-top:-30px;
    color:white;
    margin-bottom: 0px;
  }
  ion-card.kiri{
    background-color: white;
    width: 155px;
    height: 77px;
    padding-left: 8px;
    padding-top: 8px;
    margin-left: 18px;
    margin-right: 13px;
    margin-top:16px;
    border-radius: 20px;
  }
  ion-card.kanan{
    background-color: white;
    width: 155px;
    height: 77px;
    padding-left: 8px;
    padding-top: 8px;
    margin-left: 0px;
    margin-right: 0px;
    margin-top:16px;
    border-radius: 20px;
  }
  ion-card-title{
    color:black;
    font-weight: 700;
    font-size: 30px;
  }
  ion-card-subtitle{
    color: black;
    font-size: 18px;
  }
  ion-card.ikan{
    padding-top: 30px;
    padding-left: 10px;
    width: 185px;
    height: 240px;
    background-color: white;
    border-radius: 20px;
    margin-left: 10px;
    margin-right: 0px;
  }
  span.tambahan{
    font-size: 20px;
    font-weight: 400;
  }
  img.picture{
    width: 140px;
    height: 140px;
    margin-bottom: 0px;
  }
  h1.textIkan{
    text-align: left;
    font-size: 18px;
    color: black;
  }
  span.berat{
    color: #2c96f1
  }
  .menu2{
    margin-top: 20px;
    color:white;
    margin-bottom: 0px;
  }
  .kualitas{
    height: 160px;
    width: 170px;
    margin-left: 5px;
    background-color:white;
    border-radius: 20px;
    padding-left: 10px;
  }
  .text{
    color: black;
    text-align: left;
  }
  .ktitle{
    color: black;
    font-size: 40px;
    font-weight: bold;
  }
  .kopsi{
    color: black;
    font-size: 15px;
    font-weight: 400;
  }
  .khasil{
    font-size: 15px;
    color:#2c96f1
  }
  #container {
    text-align: center;
    
    position: absolute;
    left: 0;
    right: 0;
    top: 50%;
    transform: translateY(-50%);
  }
  
  #container strong {
    font-size: 20px;
    line-height: 26px;
  }
  
  #container p {
    font-size: 16px;
    line-height: 22px;
    
    color: #8c8c8c;
    
    margin: 0;
  }
  
  #container a {
    text-decoration: none;
  }
  </style>
  
