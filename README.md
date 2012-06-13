cbvtools
========

Django Class Based Views tools

from cbvtools import TemplateView, LoginRequiredView

class MyView(TemplateView):
    template_name = 'base.html'
    def get(self, request):
        data = 'hello'
        return self.render_to_response(data=data)